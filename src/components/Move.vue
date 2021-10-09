<!-- ============================== Script ============================== -->
<script setup>
import Example from '@/components/Example.vue';
const props = defineProps({
    id: {
        type: String,
        description: "unique id of this move so that it can be recognized uniquely when multiples are embedded on a single page.  Preferably the move name.",
        required: true,
    },
    bordered: {
        type: Boolean,
        body: "Renders the move within a border.",
    },
    ruled: {
        type: Boolean,
        body: "Renders the move with top and bottom horizontal rules.",
    },
    shaded: {
        type: Boolean,
        body: "Renders the move within a shaded box.",
    },
    leftLined: {
        type: Boolean,
        body: "Renders the move body with a vertical border on the left side."
    },
});
</script>

<!-- ============================== Template ============================== -->
<template>
<div :class="{
    'move': true,
    'move--bordered': bordered,
    'move--ruled': ruled,
    'move--shaded': shaded,
}">
    <div class="move__title">
        <div class="move__name"><slot name="name"/></div>
        <div class="move__example">
            <Example :id="id">
                <template v-slot:header><slot name="name"/></template>
                <template v-slot:body><slot name="example"/></template>
            </Example>
        </div>
    </div>
    <div class="move__preconditions"><slot name="preconditions"/></div>
    <div :class="{
        'move__body': true,
        'move__body--leftLined': leftLined,
    }">
        <slot name="body"/>
    </div>
</div>
</template>

<!-- ============================== Style ============================== -->
<style lang="scss" scoped>
.move {
    --indent--small: 16px; 
    --indent: 24px;

    padding: 12px 6% 12px 4%;

    @media screen and (max-width: 900px) {
        padding: 12px 4% 12px 4%;
    }

    &--bordered {
        border-radius: 8px;
        border: 1px solid var(--move-color-border, white);;
    }

    &--ruled {
        border-top: 1px solid var(--move-color-border, white);
        border-bottom: 1px solid var(--move-color-border, white);
    }

    &--shaded {
        background-color: var(--move-color-shaded, darkslategrey);
    }

    &__title {
        display: flex;
        justify-content: space-between;
        align-items: end;
    }

    &__name {
        font-size: 1.75em;
        font-weight: 900;
        line-height: 1.1em;
    }

    &__example {
        margin-top: 8px;
    }

    &__preconditions {
        font-style: italic;
        margin-left: var(--indent);
        font-size: 0.8em;

        @media screen and (max-width: 900px) {
            margin-top: 2px;
        }
    }

    &__body {
        padding-left: var(--indent);
        margin-top: 12px;

        &--leftLined {
            border-left: 1px solid var(--move-color-border, white);
            margin-left: 4px;
        }

        @media screen and (max-width: 900px) {
            padding-left: 12px;
            margin-top: 8px;

            &--leftLined {
                border-left: 1px solid var(--move-color-border, white);
            }
        }
    }
}
</style>