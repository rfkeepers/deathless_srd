<!-- ============================== Script ============================== -->
<script setup>
import Options from '@/components/Options.vue';

</script>

<!-- ============================== Template ============================== -->
<template>
<div class="core">

    <h1 class="title">
        The Master of Ceremonies
    </h1>

    <div class="spaceAbove">
        <h2 id="pbta_principles">MC Agenda</h2>
        <div class="blurb">
            <Options bullet="⇀" :options="[
                'Make the world crooked, remorseless, and hungry.',
                'Make the people layered, surprising, and real.',
                'Fill the characters\' lives with barbed hooks.',
                'Play to find out what happens.',
            ]" />
        </div>
        <br>
        You can read about each of these points individually in <router-link to="/heart">The Heart</router-link> of the game.  The overarching goal of the agenda is to provide you with a set of guiding principles.  When the world you create looks and feels and acts like what the agenda describes, then you're playing the game in the appropriate space.  Anytime you're stuck on a decision, especially when you're not sure how to move forward with a scene or what new element to introduce, turn to this list and ask, "how do I make the world feel like my agenda?"
        <br><br>
        Next are your Principles.  If the agenda is a compass to point you in the right direction, principles are a map with the roads that can take you there.  Use them to answer questions like, "how do I make the world seem hungry?" or "where do I plant these hooks?"  The Agenda and Principles both exist in the Conversation.  They are not mechanics.  A player doing this or that will not trigger a principle.  No rule will say, "use your agenda here".  This guidance is a foundation to build the rest of the game upon.
        <br><br>
        Finally, you get a list of MC Moves.  These are mechanical: a layer of rules that float on top of the conversation.  Moves describe what you are able to do.  The specific tools at your disposal for affecting change in the moment.
    </div>

    <div class="spaceAbove">
        <h2 id="pbta_principles">PBTA Principles</h2>
        <div class="blurb">
            <Options bullet="⇀" :options="[
                'Begin and end with the fiction.',
                'Address the characters before the players.',
                'Ask dangerous questions and wield the answers.',
                'Tell players the requirements or consequences, then ask.',
                'Give information freely and honestly.',
                'Think offscreen, too.',
            ]" />
        </div>
        <br>
        Many of your principles are common throughout the various PBTA games.  The wording may change a little here or there, but the underlying advice remains similar throughout.  What's advised here will help prepare the stage to showcase your other principles and agenda.

        <h4>Begin and end with the fiction</h4>
        All actions in the game should be grounded in the fiction, even when the rules are involved.  Moves aren't invoked directly.  Players should describe the things their character does in the fiction, and that fiction then triggers one of their moves.  If Sara says, "I want to Harm them, so I guess that's an Overwhelm?", take a moment to pause and discuss how that happens.  Does her character attack with a weapon?  Are they verbally dressing someone down?  What exactly does she say or do to trigger Overwhelm?  These details are important to help everyone at the table create a mental picture of how the moment plays out.  They'll also help you understand what happens to Sara's character afterward, what position they end up in and, if you have the opportunity to make a move, how you can leverage that position in your reaction.
        <br><br>
        Likewise, the outcome should also occur in the fiction.  If Sara's character slashes an opponent with their knife, the result is not simply that "your opponent takes 1 Harm".  That person just got cut up.  Where were they hit?  How badly?  How do they respond, assuming they're still alive?  Any action that instigates fictional change must result in fictional aftermath.
        <br><br>
        You're bound to this principle as much as the players.  When you use one of your own moves, make it happen in the fiction.  Disguise the consequence in a way that flows naturally from the current moment.  Don't say, "I'm going to destroy your resources", when you can say, "the paper in your cart has caught fire, one of the stray embers must have fallen inside".  Instead of, "I'm turning your safety into danger", say, "Bogan left to take a piss ten minutes ago, and he still hasn't come back.  Something is up."

        <h4>Address the characters before the players</h4>
        To keep the conversation directed at the fiction, address the players as their characters, not as people in control of characters.  When you ask a player what their character does, you're having a conversation about some separate fictional event, and creating a story by proxy.  When you say the character's name and ask what they do, the resulting conversation becomes the fiction, and is the story itself.
        <br><br>
        Inversely, when you need to talk about things outside of the fiction- to address safety concerns, check in with the group, or whatever else- you have a clear divide between fiction and reality.  Address the players at this time, not the characters.

        <h4>Ask dangerous questions and wield the answers</h4>
        Because you, like the players, are playing to find out what happens, you can't be expected to know everything about the fiction surrounding you.  Be curious, and be a fan of what your players might have ideas for.  Ask them what they think of the situation, about themselves and each other.  Ask them what they're scared might happen.  Be bold and ask about topics beyond their own character: why is the world this way?  What do the people here think of their rulers?  What name do the people here pray to, and is that psychopomp alive?  And, of course, always ask them, "what do you do?"
        <br><br>
        Once you have your answers, wield them.  Change the world.  Manifest adversaries and interference.  Bring those answers to life in small and large ways both.  The players may not control the world like you do, but by planting the seeds of their ideas you encrich the fiction in ways that everyone cares about.  And when everyone cares about the fiction, they've given it teeth to bite back at them.

        <h4>Give information freely and honestly</h4>
        All roleplay deals with the control of knowledge in some form or another, but remember your agenda: play to find out what happens, not play to trickle information down to the players.  Duplicity and secrets are at odds with the nature of the converation, and tend to sow contention between the players and MC.  Trust your players to handle an open flow of information.  Help them be are aware of, and buy into, the dramatic irony of the situation.

        <h4>Think offscreen, too</h4>
        The actions and reactions of the world mustn't always occur in the immediate space around the players' characters.  The world lives and breathes even when it isn't observed.  What are people scheming in the background?  How do they maneuver their advantage?  Things are constantly changing behind the characters' backs.  Don't be afraid to make changes offscreen while the characters act successfully onscreen.
    </div>

    <div class="spaceAbove">
        <h2 id="deathless_principles">Deathless' Principles</h2>
        <div class="blurb">
            <Options bullet="⇀" :options="[
                'Fill the story with frequent strife and transient relief.',
                'Deal in costly decisions, misfortune, and trouble that always comes looking.',
                'Give nothing away freely.',
                'Make fraught situations deadly.',
                'Use the unnatural to talk about the human.',
                'Pursue accountability for the actions commmitted.',
            ]" />
        </div>

        <h4>Fill the story with frequent strife and transient relief</h4>
        <h4>Deal in costly decisions, misfortune, and trouble that always comes looking</h4>
        <h4>Give nothing away freely</h4>
        <h4>Make fraught situations deadly</h4>
        <h4>Use the unnatural to talk about the human</h4>
        <h4>Pursue accountability for the actions commmitted</h4>
        <h4>Give information freely and honestly</h4>
    </div>

    <div class="spaceAbove">
        <h2 id="mc_moves">MC Moves</h2>
        While the players and MC both have moves, yours work in a very different way than theirs.  You never roll, and your moves never fail.  When you say that something happens, it happens.  And whatever that is, it happens in the fiction.  This is part of "Never speaking the name of your move".  What your moves allow you to do is to make statements that are fictionally true, so long as they are backed by a move.  Ie:
        <br><br>
        Although your moves describe what you're allowed to do, they do so in broad strokes and intentionally leave much to the imagination.  This is because they're not singular in purpose.  Not solely for retaliating or punishing the players.  They are, fundamentally, tools to keep the story interesting and tense.  Sometimes this Many times you'll need them to prod a stalled conversation or fine tune the tension by, say, turning safety to danger, or advancing an antagonist's agenda.
        <br><br>

        <h3>When To Make Moves</h3>
        <h4>After a player move allows it</h4>
        Most player moves in the game will describe what to do on a Successful or Partially successful roll, but won't say what to do on a Miss.  Other times the move will state that you get to make a move in addition to the other outcomes.  In both cases you are allowed to make a move "as hard as you want".  As hard as you want doesn't need to mean you assign the maximum punishment to the character, although you are allowed to do so.  It means your move can affect them as directly or indirectly as you please.
        <br><br>
        On the topic of directness, Deathless functions best when characters fail forward.  That is, a Missed move doesn't need to prevent them from achieving their goals, especially since that often stalls the momentum.  In most situations it is better to let the character succeed, and then come at them sideways with a new problem.

        <h4>When everyone looks at you to see what happens next</h4>
        Anytime the players aren't moving the scene forward on their own, they're probably looking at you to do it for them.  Maybe this is because the conversation stalled.  Maybe something new is in the scene and they aren't sure how to approach it.  Maybe, most simply, they just made their own move and are curious to see what happens next.  Whatever the cause, this is your opportunity to push things in a certain direction, to set up new tension and danger, and keep the scene moving forward.

        <h4>If given a golden opportunity</h4>
        A golden opportunity happens when the players leave a previous event unaddressed.  If you put danger or opposition in the scene, and the players don't do anything about it, you now have a golden opportunity to follow through on that setup.

        <h3>After Making A Move</h3>
        Once you've made a move, always ask the players, "what do you do?"  This is the most essential part of the conversation.  Your moves are your way of abiding your principles and fulfilling your agenda.  The players have their own agenda, and must get their own opportunity to act.

        <h3>Moves</h3>
        <div class="blurb">
            <Options bullet="⇀" :options="[
                'Reveal an unwelcome truth',
                'Turn safety to danger',
                'Make their behavior cause more trouble than it solves',
                'Harm them with pain, insult, or injury',
                'Remind them of their place in the world',
                'Compel them to complicate the situation',
                'Manipulate loyalties or turn them against each other',
                'Destroy resources',
                'Tug at the strings of Entanglements',
                'Advance an antagonist\'s agenda, on or offscreen',
                'Offer a painful opportunity',
            ]" />
        </div>

        <h4>Reveal an unwelcome truth</h4>
        <h4>Turn safety to danger</h4>
        <h4>Make their behavior cause more trouble than it solves</h4>
        <h4>Harm them with pain, insult, or injury</h4>
        <h4>Remind them of their place in the world</h4>
        <h4>Compel them to complicate the situation</h4>
        <h4>Manipulate loyalties or turn them against each other</h4>
        <h4>Destroy resources</h4>
        <h4>Tug at the strings of Entanglements</h4>
        <h4>Advance an antagonist's agenda, on or offscreen</h4>
        <h4>Offer a painful opportunity</h4>
    </div>

</div>
</template>

<!-- ============================== Style ============================== -->
<style lang="scss" scoped>
$varname: 1;
.core {
    padding-bottom: 24px;
}
</style>