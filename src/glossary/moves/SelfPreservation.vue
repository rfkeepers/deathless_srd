<!-- ============================== Script ============================== -->
<script setup>
import Move from "@/components/Move.vue";

const name = 'Self-Preservation';
</script>

<!-- ============================== Template ============================== -->
<template>
<Move id="self_preservation" leftLined>
    <template v-slot:name>{{name}}</template>
    <template v-slot:preconditions>( Embodied )</template>
    <template v-slot:body>
        When you <b>stay hidden while you let danger or harm befall someone</b> whom it would benefit you to help, remove a Condition or gain 2 Resilience.
    </template>
    <template v-slot:example>
        <h3 class="lineTo indent">Design Thoughts</h3>
        Finally, we get to the cowardice of the shadewalker persona.
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