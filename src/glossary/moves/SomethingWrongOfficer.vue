<!-- ============================== Script ============================== -->
<script setup>
import Move from "@/components/Move.vue";
import Roll from "@/components/Roll.vue";
import SHPM from "@/components/SHPM.vue";

const name = 'Something Wrong, Officer?';
</script>

<!-- ============================== Template ============================== -->
<template>
<Move id="something_wrong_officer" leftLined>
    <template v-slot:name>{{name}}</template>
    <template v-slot:body>
        When you <b>dissuade a person of law or authority</b> from getting involved, <Roll resolve/>.
        <SHPM :options="[
            'They give you the benefit of the doubt and leave you alone.',
            'They\'re hesitant and will keep an eye on things, but won\'t jump in until someone gives them a reason.',
        ]" />
    </template>
    <template v-slot:example>
        <h3 class="lineTo indent">Design Thoughts</h3>

        <h3 class="lineTo indent">In Play</h3>
        <div class="playExample miniBorder">
        <p>Skipping play examples for now.</p>
        </div>
    </template>
</Move>
</template>

<!-- ============================== Style ============================== -->
<style lang="scss" scoped>
</style>