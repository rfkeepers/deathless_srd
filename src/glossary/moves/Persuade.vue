<!-- ============================== Script ============================== -->
<script setup>
import Move from "@/components/Move.vue";
import Options from "@/components/Options.vue";
import Roll from "@/components/Roll.vue";

const name = 'Persuade';
</script>

<!-- ============================== Template ============================== -->
<template>
<Move id="persuade" leftLined>
    <template v-slot:name>{{name}}</template>
    <template v-slot:body>
        When you <b>press an NPC for something</b> they wouldn't easily agree to, <Roll glamour/>.  <em>S:</em> They will tell you the most effective way to compel them- if there is a way- otherwise they'll decline your request peacefully.  <em>P:</em> They need extra convincing- if they can be convinced; either the MC will pick an option from the list or they will reject your request in a noisy, aggressive, destructive, or alarming manner.
        <Options bullet="⇀" :options="[
            'Give them substantial payment up front.',
            'Allow them to request something of you in turn.',
            'Prove you\'re willing to hurt them.',
            'Nothing. But they\'ll make sure everyone, or the right person, hears about this.',
            'Nothing. But you\'ve brought risk or harm to someone else as a result.',
        ]" />
        <br>
        When you press a fellow PC to do things after they have given valid reasons to not get involved, they may shut you down once and for all or let you roll for it.  If they let you roll, <Roll n=3 dice/>.  <em>S:</em> They take 1 Resilience.  <em>P:</em> They choose 1.  <em>M:</em> They choose 2.  
        <Options bullet="⇀" :options="[
            'Require a Debt.  When they call in the Debt to gain a favor or payment, if you fail to uphold your end of the agreement add one mark of Abyss.',
            'They take 2 Resilience.',
            'They erase one mark of Abyss.',
            'You must pledge Loyalty to them.  This Entanglement must state an end condition.',
        ]" />
    </template>
    <template v-slot:example>
        <h3 class="lineTo">Design Thoughts</h3>
        I have a conflicted relationship with persuasion moves.  That is, how do you maintain an npc's independent motivations if you let any old roll make them, "just do the thing you ask"?  Works fine in a game that doesn't hinge as much on behavioral conflicts.  So I ended up writing an overbearing move like this to make the ends meet.  I do see like persuasion moves overall.  They're one of the rules that help give the MC plausible deniability over how they're making the npcs behave.  But writing one nuance seems to highlight all the nuances that got ignored.
        <h3 class="lineTo">In Play</h3>
        <div class="playExample miniBorder">
        <p>"Like I said," the MC reiterates, playing the part of the Consul, "you haven't brought rigorous evidence.  Certainly not enough to warrant action against a person as important as the Baron."</p>
        <p>"We told you where to find people who'd give evidence under oath!"</p>
        <p>"You know where to find two ruffians willing to speak?  Wonderful, bring them here yourselves! Let them speak!  I'll give them the floor.  I swear, if I have to hear one more claim like this today."</p>
        <p>"Hold up," Ewan say, "one more?  Someone else told you this?"</p>
        <p>"The Consul clams up real quick," says the MC.</p>
        <p>"We're not stopping here," Ewan continues.  "What, are you taking payment from the Baron, too?"</p>
        <p>"It's a delicate matter"</p>
        <p>"Who?" Ewan asks, "who was it?  If you really aren't in the Baron's pocket then I sure as hell hope you think his business is as vile as we do.  You need better evidence?  Fine, tell us who else is talking to you.  Just that.  We can find them.  We can get you evidence."  Ewan pauses, waits for the MC to say something, then sighs, "what will it take to get a name?"</p>
        <p>"Roll to Persuade this guy," the MC tells him.  Ewan rolls a Success.  "Okay," the MC begins, "the Consul makes a curt nod towards the door and waits for one of you to close it.  'You want a name?  I want a reason to move this to action.  You have three hours to bring me your informants.  And before you accuse me of being severe you should know that the Baron has ears here- with all your shouting you'll be lucky if what I've afforded you is long enough.  I need people who know names, who know places, who know where I can find paperwork.  Bring them to me and you'll get your name.'."</p>
        </div>
    </template>
</Move>
</template>

<!-- ============================== Style ============================== -->
<style lang="scss" scoped>
</style>