<!-- ============================== Script ============================== -->
<script setup>
    import Move from '@/components/Move.vue';
    import Options from "@/components/Options.vue";

</script>

<!-- ============================== Template ============================== -->
<template>
    <h1>Obsession</h1>
    While hopes and dreams often provide simple aspiration, an obsession can overwhelm the motivation for living altogether.  Taking on an Obsession is entirely up to the player.  No other character may ask you to do so, the MC cannot, nor can a move or compel force you into it.  But they shouldn't be taken lightly, either.  Once acknowledge, it can be very difficult to clear your mind of its Obsessions without resolving them entirely.
    <br><br>
    Examples:
    <Options bullet="⇀" :options="[
        'There is nothing more rotten than the sale of a human life.  I will put an end to the trafficking ring run by the Baron de RoseFitz.',
        'Demonic blood is rare and excuisitely valuable.  Draining the demon-boar of Sekkerdi would make enough lucre to live for generations in splendor.',
        'I have a son, Bergen; a product of my own loins on the eve of my death.  This long existence will turn me hollow if I never meet him.',
    ]" />
    <br><br>
    <Move id="become_obsessed" ruled shaded>
        <template v-slot:name>Become Obsessed</template>
        <template v-slot:body>
            When something <b>grips you completely and refuses to leave your mind</b>, you have a choice: shut it out and never give it your attention again, or dedicate yourself to chasing it down at all costs.  If you resist the urge, you're free and can try to steer clear of it in the future.  If you give in, write a new Obsession that describes whatever captivated you, and what you intended to do about it.
        </template>
        <template v-slot:example>
        <h3 class="lineTo">Design Thoughts</h3>
            todo
        <h3 class="lineTo">In Play</h3>
        <div class="playExample miniBorder">
            <p>"todo", the author says.</p>
        </div>
        </template>
    </Move>
    <h2>Maintaining Obsession</h2>
    <Options bullet="❍" :options="[
        'When you earnestly go out of your way to endure significant Harm, hardship, or danger for the sake of making progress towards your obsession- whether or not you are successful- erase a mark of Abyss.  This can only occur once per scene, independent of the number of Entanglements involved.',
    ]" />
    <h2>Completion</h2>
    <Options bullet="❍" :options="[
        'If something in the world changes and the source of your Obsession, or your ability to pursue it, disappears, erase the Entanglement and answer the questions below.  If you answered \'yes\' to any of those questions, erase 2 marks of Abyss.  If you did not, gain 2 marks of Abyss.'
    ]">
        <template v-slot:subslot-0>
            <Options bullet="⇀" :options="[
                'If your obsession was a question, were you able to answer it to some satisfaction, even if not completely?',
                'If your obsession was an opportunity, were you able to capitalize on it to some satisfaction, even if only a little bit?',
                'If your obsession was a project, were you able to affect or progress it meaningfully, even if only incrementally?',
            ]" />
        </template>
    </Options>
    <h2>Failure</h2>
    <Options bullet="❍" :options="[
        'When you turn down a clear opportunity to pursue your Obsession, add a mark of Abyss.  The MC will always give you a warning when you are about to pass up a clear opportunity.',
        'If you do any of the following with clear intent: endure prolonged separation from your Obsession or persistently decline the opportunity to make progress towards it, erase the Obsession and mark the Abyss.  The MC will always give you a warning if your actions would default on the Entanglement, and your choice to defy this warning is what counts as clear intent.'  
    ]" />
    <h2>Abandonment</h2>
    <Options bullet="❍" :options="[
        'If you find yourself in a situation where chasing your Obsession has become distasteful, disturbing, or self destructive, your only out is to find closure, somehow.  Obsession is difficult like that, you don\'t have the power to tell yourself to stop.  Instead, you may propose to change the terms.  If the table agrees with your proposal, you may rewrite your Obsession at no cost.  This may not alter the type of Entanglement.'
    ]" />
    <br><br>
    &nbsp;
</template>

<!-- ============================== Style ============================== -->
<style lang="scss" scoped>
</style>