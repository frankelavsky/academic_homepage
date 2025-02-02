---
layout: post
title: "Streetrat: A Thief's Text Adventure"
slug: streetrat
tags:
  - video game
  - text game
  - text adventure
description: I made a text adventure game where you play a thief who is hoping to get their first, real, big break.
---

In my class "Programming for Game Designers" (which I am taking for fun as my final course in my PhD), our first major project is to design, code, playtest, and refine a text-based adventure game. We are using [textadventures](https://textadventures.co.uk/) and their visual script editor/IDE [Quest](https://github.com/textadventures/quest) for the assignment.

If you've never played a text adventure before, we were assigned [Jacqueline, Jungle Queen!](https://textadventures.co.uk/games/view/vpf7vh9mfusdg4mta1u76g/jacqueline-jungle-queen) to play in order to get acquainted. Basically, text adventure games take text input from the player and an interactive story unfolds. Some are designed with multiple endings, others are filled with tricky puzzles to solve. It's a great format of game.

## How did I make it?

If you want to know how I designed and play-tested Streetrat, then check out my [previous blog post](https://www.frank.computer/blog/2025/01/play-testing-streetrat.html), where I break my process down.

## Where can I play it?

[Streetrat has been officially released on textadventures](https://textadventures.co.uk/games/view/2rop_rny2ke_tgzfp_da6g/streetrat).

Give it a try! I'd love to hear your feedback. It can probably be beaten in 15 to 30 minutes (but in much less time if you know the spoilers!).

## Playthrough

My thorough playthrough is detailed below. In this session I try out every major command at least once, on at least every interactive object in the game, and visit every location. I also end the game with a perfect score. Note: This walkthrough is a copy+paste of the HTML from the game's text log output.

With extra paragraph breaks removed, pasting the text below into [google docs results in a 28-page adventure](https://docs.google.com/document/d/1b0FQZwSLakh9c1cDO7kwjeINC7P1St_SNza8Nh-3DBI/edit?usp=sharing)! That's pretty neat to think about. 28 pages is a decent amount of writing! Now I wish I had done this sooner though, because I can see that I've misspelled "chails" (chains), "aquaducts" (aqueducts), "purfumes" (perfumes), "entrace" (entrance), "mischeivious" (mischeivous), "keyhold" (keyhole), and "unkept" (unkempt). Oof! Too bad quest doesn't have built-in spell checking.

<details>
    <summary>Open playthrough (<i>spoiler warning</i>)</summary>
    <div id="gameContent" style="width: 700px">
      <div id="gamePanelSpacer" style="height: 0px"></div>
      <div id="divOutput" style="margin-top: 20px">
        <div id="outputData" style="display: none" data-divcount="257" data-currentdiv="#divOutputAlign257"></div>
        <div id="divOutputAlign1" style="text-align: left" class="section1"></div>
        <div id="divOutputAlign2" style="text-align: left" class="section1 title"></div>
        <div id="divOutputAlign3" style="text-align: center" class="section1 title">
          <h2><span>Streetrat</span></h2>
        </div>
        <div id="divOutputAlign4" style="text-align: left" class="section1 title"></div>
        <div id="divOutputAlign5" style="text-align: center" class="section1 title"><span>by F.E.</span><br /></div>
        <div id="divOutputAlign6" style="text-align: left" class="section1 title">
          <span><div style="margin-top: 20px"></div></span><br />
        </div>
        <div id="divOutputAlign7" style="text-align: left" class="section1">
          <span>Created by Frank Elavsky, a student at Carnegie Mellon University, for a class project.</span><br /><span><a href="https://www.frank.computer/blog/2025/01/play-testing-streetrat.html">Frank's process is detailed on his blog.</a></span
          ><br /><span
            ><br />You're an urchin, a thief, a regular streetrat. You've been scurrying around the streets of this dusty, burning-hot city for years now after being kicked out of the orphanage. You mostly try to lay low, but lately the city guard have been increasing in number. It's harder and
            harder to get away with what you used to. It's probably time to plan a proper heist or something and get out of this town for good. </span
          ><br /><span>But first... *your stomach growls right on cue* you need to get some breakfast.</span><br /><span><img src="https://www.frank.computer/images/streetrat.JPG" alt="Streetrat logo shown over a pile of gold and jewelry" /></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink1" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span>, a
            <span id="verblink2" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span>, a
            <span id="verblink3" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink4" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink5" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink6" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign8" style="text-align: left" class=""></div>
        <div id="divOutputAlign9" style="text-align: left" class="section2">
          <span></span><br /><span>&gt; examine poor woman</span><br /><span
            >An older, poor woman who is shuffling about in the crowd. She is probably getting into some kind of trouble, just like you. You make eye contact for a moment and she gives you a mischeivious grin with a few teeth missing.</span
          ><br />
        </div>
        <div id="divOutputAlign10" style="text-align: left" class=""></div>
        <div id="divOutputAlign11" style="text-align: left" class="section3">
          <span></span><br /><span>&gt; x monkey</span><br /><span
            >A lanky monkey wearing a little purple vest. It always seems to be in the market. You figure it used to be (or still is) someone's pet, since it is so comfortable around people and has a sense of fashion. It doesn't pay any attention to you as it swings about between the
            stalltops.</span
          ><br />
        </div>
        <div id="divOutputAlign12" style="text-align: left" class=""></div>
        <div id="divOutputAlign13" style="text-align: left" class="section4">
          <span></span><br /><span>&gt; x bakery</span><br /><span>The front counter of the bakery, which extends into the market.</span><br /><span
            >It contains a <span id="verblink7" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink8" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>.</span
          ><br />
        </div>
        <div id="divOutputAlign14" style="text-align: left" class=""></div>
        <div id="divOutputAlign15" style="text-align: left" class="section5">
          <span></span><br /><span>&gt; x baker</span><br /><span
            >A beautifully large baker, your favorite baker in the market in fact. They are standing with their back turned to you, clearly working hard on something behind the counter as their large arms roll and push and their shoulders lift and fall rhythmically. They're completely engrossed in
            their work.</span
          ><br />
        </div>
        <div id="divOutputAlign16" style="text-align: left" class=""></div>
        <div id="divOutputAlign17" style="text-align: left" class="section6">
          <span></span><br /><span>&gt; x baguette</span><br /><span
            >A freshly baked baguette. The bread's crust is perfectly golden and you can smell how good it must taste. The steam rising off of it means it must have just been taken out of the oven and put on display. Your mouth waters the more you look at it.</span
          ><br />
        </div>
        <div id="divOutputAlign18" style="text-align: left" class=""></div>
        <div id="divOutputAlign19" style="text-align: left" class="section7">
          <span></span><br /><span>&gt; x guard</span><br /><span
            >A fearsome, tall guard with chainmail armor and a closed-visor helmet stands about half of a block away from the bakery, looking into the market square. They're standing almost perfectly straight but you can see their eyes busily darting about. As you walk past them, you can hear the
            intensity of their breathing through their visor, like steam from a dragon's mouth. They have one hand resting on a sword's pommel, which is sheathed on their belt. You can tell by the patina on the sword handle's leather that they've seen a lot of action. This guard is not to be messed
            with.</span
          ><br />
        </div>
        <div id="divOutputAlign20" style="text-align: left" class=""></div>
        <div id="divOutputAlign21" style="text-align: left" class="section8">
          <span></span><br /><span>&gt; east</span><br /><span></span><br /><span>You are in the Courtyard.</span><br /><span
            >You can see a <span id="verblink9" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace guards" data-verbs="Look at/Misdirect">palace guards</span>, a
            <span id="verblink10" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="rich man" data-verbs="Look at/Speak to/Misdirect">rich man</span>, a
            <span id="verblink11" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace gate" data-verbs="Look at">palace gate</span> and a
            <span id="verblink12" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger pen" data-verbs="Look at">tiger pen</span> (containing a
            <span id="verblink13" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>).</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit2" data-command="go west">west</span>.</span><br /><span
            >The courtyard outside of the palace is beautifully well-kept and green with plenty of shade. The aquaducts bring water in to keep this area green, unlike the rest of the city. The trees and bushes smell crisp and clean and the warm air from the south sometimes passes through. The
            sandstone under your feet even has intricate carvings. People old, young, rich, and poor all care about this place. People usually speak in quieter voices here than the market. There are many places to sit and lounge, even some stone tables for people to gather around. There is a
            peacefulness here.</span
          ><br />
        </div>
        <div id="divOutputAlign22" style="text-align: left" class=""></div>
        <div id="divOutputAlign23" style="text-align: left" class="section9">
          <span></span><br /><span>&gt; x guards</span><br /><span
            >A pair of guards standing at the entrace to the palace. They are wearing shining, full-body plated armor that is covered in white silk cloaks with golden trim. They each have long polearms with wavy blades at the end. They must be cooking alive in that gear under the sun all day, but
            they do look pretty awesome.</span
          ><br />
        </div>
        <div id="divOutputAlign24" style="text-align: left" class=""></div>
        <div id="divOutputAlign25" style="text-align: left" class="section10">
          <span></span><br /><span>&gt; x rich</span><br /><span
            >This guy is a grade-A jerk, you can tell just by how he stands there, doing nothing. He has a long, thin moustache that he is swirling in his finger as he stares into the tiger pen, mumbling something to himself. His nails are clean, hair is shiny, skin is powdered, clothes look brand
            new, and when you get close, he smells like those expensive soaps you're not even allowed near in the market. He's wearing a long robe with all sorts of fine patterns sewn in. Loosely tied to a sash on his waist is a small
            <span id="verblink14" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>.</span
          ><br />
        </div>
        <div id="divOutputAlign26" style="text-align: left" class=""></div>
        <div id="divOutputAlign27" style="text-align: left" class="section11"><span></span><br /><span>&gt; x purse</span><br /><span>A small, velvet purse with a golden trimmed clasp. You can tell there is something inside of it by how it hangs with weight.</span><br /></div>
        <div id="divOutputAlign28" style="text-align: left" class=""></div>
        <div id="divOutputAlign29" style="text-align: left" class="section12">
          <span></span><br /><span>&gt; x gate</span><br /><span>A pair of beautiful doors that lead into the palace. They are wide, tall, and made of some kind of gilded metal. You might not even be able to open them if you tried. They probably weigh more than a hippo each.</span><br />
        </div>
        <div id="divOutputAlign30" style="text-align: left" class=""></div>
        <div id="divOutputAlign31" style="text-align: left" class="section13">
          <span></span><br /><span>&gt; x pen</span><br /><span
            >A large, walled off area that is about 1 story below the ground. If you walk to the edge of the wall, you can look down inside. Inside the pen is a grassy hill and several trees, a small pond, and a little cave near the back of the hill. A thick ship-rope hangs from the tree with a
            leather ball tied to the end, dangling just above the ground. Clearly the tiger enjoys playing with it because it is covered in scratches and gouges and has a heavy patina worn in.</span
          ><br /><span>It contains a <span id="verblink15" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>.</span><br />
        </div>
        <div id="divOutputAlign32" style="text-align: left" class=""></div>
        <div id="divOutputAlign33" style="text-align: left" class="section14"><span></span><br /><span>&gt; x tiger</span><br /><span>A majestic, muscular tiger. It is currently napping on the sunny side of the hill in its pen.</span><br /></div>
        <div id="divOutputAlign34" style="text-align: left" class=""></div>
        <div id="divOutputAlign35" style="text-align: left" class="section15"><span></span><br /><span>&gt; take purse</span><br /><span>You can't take it.</span><br /></div>
        <div id="divOutputAlign36" style="text-align: left" class=""></div>
        <div id="divOutputAlign37" style="text-align: left" class="section16">
          <span></span><br /><span>&gt; w</span><br /><span></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink16" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span>, a
            <span id="verblink17" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span>, a
            <span id="verblink18" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink19" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink20" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink21" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign38" style="text-align: left" class=""></div>
        <div id="divOutputAlign39" style="text-align: left" class="section17">
          <span></span><br /><span>&gt; take bread</span><br /><span
            >You take the baguette without being seen by the baker and slip into a nearby alley. You stuff your face with the steaming, hot bread. <br /><br />As you're chomping down, you hear heavy, clomping footsteps approaching and the sound of clinking metal chails. "Uh oh," you think to
            yourself. "Not again..." <br /><br />Suddenly two guards turn the corner. You drop the crust of the last couple bites on the ground and back up, hands in the air, and an awkward smile on your face as you finish chewing. Before you can speak, your back bumps into something large.
            <br /><br />You turn around just as the three guards seize you and take you off to jail.</span
          ><br /><span></span><br /><span>You are in a Jail Cell.</span><br /><span
            >You can see a <span id="verblink22" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="grate" data-verbs="Look at/Pick">grate</span>, a
            <span id="verblink23" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="jail guard" data-verbs="Look at/Speak to/Misdirect">jail guard</span> and a
            <span id="verblink24" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="chair" data-verbs="Look at">chair</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="Jail Exit" data-command="go west">west</span>.</span><br /><span
            >A dark, damp underground holding area under the palace, lit by torchlight. This is where they take the minor criminals and it's the best jail in the city. The really bad criminals go to the dungeon at the edge of town where everyone gets sick and the guards are mean. This jail exists
            because the lord set lenient laws in an attempt to distance his reputation from his deeply cruel father (the messed-up guy who ruled before him). As a result, petty theft results in a 1-day hold in the palace jail overnight instead of losing a hand by sword on the spot. You got into
            theft just in time. One generation sooner and you'd already have lost dozens of hands to the local guards. They catch you stealing bread pretty much every other day now.</span
          ><br />
        </div>
        <div id="divOutputAlign40" style="text-align: left" class=""></div>
        <div id="divOutputAlign41" style="text-align: left" class="section18"><span></span><br /><span>&gt; x grate</span><br /><span>An iron grate door. If only you were really skinny, you could just squeeze out between the bars.</span><br /><span>It is locked.</span><br /></div>
        <div id="divOutputAlign42" style="text-align: left" class=""></div>
        <div id="divOutputAlign43" style="text-align: left" class="section19">
          <span></span><br /><span>&gt; x guard</span><br /><span
            >A guard sits slumped in a chair, spear in one hand and a book in their other. They look bored out of their mind as they read; it must not be a very good book. Every few minutes they turn a new page by awkwardly resting their spear handle on their shoulder to free their other hand for a
            moment.</span
          ><br />
        </div>
        <div id="divOutputAlign44" style="text-align: left" class=""></div>
        <div id="divOutputAlign45" style="text-align: left" class="section20">
          <span></span><br /><span>&gt; x chair</span><br /><span>A plain, wooden chair.</span><br /><span><br />Oof... there really is nothing to do right now.</span><br />
        </div>
        <div id="divOutputAlign46" style="text-align: center" class="section20">
          <span><br />You have learned how to <b>WATCH</b>.<br /></span><br />
        </div>
        <div id="divOutputAlign47" style="text-align: left" class="section20">
          <span
            >Use <span id="verblink25" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="watch" data-command="watch">watch</span> as a command to see if circumstances change wherever you are. Sometimes new opportunities present themselves, if you're observant
            enough.</span
          ><br />
        </div>
        <div id="divOutputAlign48" style="text-align: left" class=""></div>
        <div id="divOutputAlign49" style="text-align: left" class="section21"><span></span><br /><span>&gt; w</span><br /><span>You can't leave while you're still in this cell (that's probably the whole point of this "jail" thing anyway).</span><br /></div>
        <div id="divOutputAlign50" style="text-align: left" class=""></div>
        <div id="divOutputAlign51" style="text-align: left" class="section22">
          <span></span><br /><span>&gt; watch</span><br /><span
            >You wait for a while, listening to the guard turn the pages in their book. Eventually they get up and wordlessly walk out of the room for the changing of the guard. Nobody comes back to take their place. It must be meal time. The silence is a bit unnerving. You're the only soul in the
            jail right now, all alone.</span
          ><br />
        </div>
        <div id="divOutputAlign52" style="text-align: left" class=""></div>
        <div id="divOutputAlign53" style="text-align: left" class="section23"><span></span><br /><span>&gt; w</span><br /><span>You can't leave while you're still in this cell (that's probably the whole point of this "jail" thing anyway).</span><br /></div>
        <div id="divOutputAlign54" style="text-align: left" class=""></div>
        <div id="divOutputAlign55" style="text-align: left" class="section24"><span></span><br /><span>&gt; open grate</span><br /><span>You can't open it.</span><br /></div>
        <div id="divOutputAlign56" style="text-align: left" class=""></div>
        <div id="divOutputAlign57" style="text-align: left" class="section25"><span></span><br /><span>&gt; unlock grate</span><br /><span>You can't unlock it.</span><br /></div>
        <div id="divOutputAlign58" style="text-align: left" class=""></div>
        <div id="divOutputAlign59" style="text-align: left" class="section26">
          <span></span><br /><span>&gt; watch</span><br /><span
            >Eventually the guards change shifts and the new guard bring you a small bowl of gruel. You drink it. A little while later, the new guard comes back to your door and lets you out. You know the drill by now. They lead you back to the market. </span
          ><br /><span>"Please stop getting into trouble. You know we are all tired of this." They sigh loudly and walk off back in the direction of the palace.</span><br /><span></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink26" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span>, a
            <span id="verblink27" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span>, a
            <span id="verblink28" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink29" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink30" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink31" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign60" style="text-align: left" class=""></div>
        <div id="divOutputAlign61" style="text-align: left" class="section27">
          <span></span><br /><span>&gt; watch</span><br /><span
            >You wait and watch the crowd. And after relaxing your eyes, you notice a twinkle in the corner of your eye. You turn and watch the monkey swiftly pick a golden pocket watch from someone's pockets and slip it into their vest pocket.</span
          ><br />
        </div>
        <div id="divOutputAlign62" style="text-align: center" class="section27">
          <span><br />You learn how to <b>PICK</b> from pockets, purses, and other things.<br /></span><br />
        </div>
        <div id="divOutputAlign63" style="text-align: left" class="section27">
          <span
            >Use <span id="verblink32" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="pick">pick</span> to try to sneakily take items. This works on things like the
            <span id="verblink33" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span>'s
            <span id="verblink34" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pouch" data-verbs="Look at/Pick">pouch</span> or the
            <span id="verblink35" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span>'s
            <span id="verblink36" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pocket" data-verbs="Look at/Pick">pocket</span> (which you've just now noticed). Just be careful! You still might get caught...</span
          ><br />
        </div>
        <div id="divOutputAlign64" style="text-align: left" class=""></div>
        <div id="divOutputAlign65" style="text-align: left" class="section28">
          <span></span><br /><span>&gt; watch</span><br /><span>You wait and watch the monkey swinging about, picking more pockets. People are bustling and hustling, coming and going. It's a lively scene; peaceful in its own way.</span><br />
        </div>
        <div id="divOutputAlign66" style="text-align: left" class=""></div>
        <div id="divOutputAlign67" style="text-align: left" class="section29"><span></span><br /><span>&gt; r</span><br /><span>I don't understand your command.</span><br /></div>
        <div id="divOutputAlign68" style="text-align: left" class=""></div>
        <div id="divOutputAlign69" style="text-align: left" class="section30">
          <span></span><br /><span>&gt; e</span><br /><span></span><br /><span>You are in the Courtyard.</span><br /><span
            >You can see a <span id="verblink37" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace guards" data-verbs="Look at/Misdirect">palace guards</span>, a
            <span id="verblink38" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="rich man" data-verbs="Look at/Speak to/Misdirect">rich man</span> (containing a
            <span id="verblink39" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>), a
            <span id="verblink40" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace gate" data-verbs="Look at">palace gate</span> and a
            <span id="verblink41" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger pen" data-verbs="Look at">tiger pen</span> (containing a
            <span id="verblink42" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>).</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit2" data-command="go west">west</span>.</span><br /><span
            >The courtyard outside of the palace is beautifully well-kept and green with plenty of shade. The aquaducts bring water in to keep this area green, unlike the rest of the city. The trees and bushes smell crisp and clean and the warm air from the south sometimes passes through. The
            sandstone under your feet even has intricate carvings. People old, young, rich, and poor all care about this place. People usually speak in quieter voices here than the market. There are many places to sit and lounge, even some stone tables for people to gather around. There is a
            peacefulness here.</span
          ><br />
        </div>
        <div id="divOutputAlign70" style="text-align: left" class=""></div>
        <div id="divOutputAlign71" style="text-align: left" class="section31"><span></span><br /><span>&gt; watch</span><br /><span>You wait and relax for a while in the shade of some large palms, watching the tiger continue to nap. No new opportunities present themselves.</span><br /></div>
        <div id="divOutputAlign72" style="text-align: left" class=""></div>
        <div id="divOutputAlign73" style="text-align: left" class="section32">
          <span></span><br /><span>&gt; w</span><br /><span></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink43" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span> (containing a
            <span id="verblink44" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pouch" data-verbs="Look at/Pick">pouch</span>), a
            <span id="verblink45" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span> (containing a
            <span id="verblink46" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pocket" data-verbs="Look at/Pick">pocket</span>), a
            <span id="verblink47" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink48" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink49" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink50" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign74" style="text-align: left" class=""></div>
        <div id="divOutputAlign75" style="text-align: left" class="section33">
          <span></span><br /><span>&gt; pick pouch</span><br /><span>You take some <span id="verblink51" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu" data-elementid="lint" data-verbs="Look at/Use/Drop">lint</span>.</span><br /><span
            >You take a <span id="verblink52" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu" data-elementid="hairpin" data-verbs="Look at/Use/Drop">hairpin</span>.</span
          ><br />
        </div>
        <div id="divOutputAlign76" style="text-align: left" class=""></div>
        <div id="divOutputAlign77" style="text-align: left" class="section34">
          <span></span><br /><span>&gt; pick pocket</span><br /><span>You take a <span id="verblink53" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pebble" data-verbs="Look at/Use/Drop">pebble</span>.</span><br /><span
            >You take a <span id="verblink54" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu" data-elementid="golden pocket watch" data-verbs="Look at/Use/Drop">golden pocket watch</span>. <i>Score!</i></span
          ><br />
        </div>
        <div id="divOutputAlign78" style="text-align: left" class=""></div>
        <div id="divOutputAlign79" style="text-align: left" class="section35"><span></span><br /><span>&gt; x lint</span><br /><span>Eww, some pocket lint.</span><br /></div>
        <div id="divOutputAlign80" style="text-align: left" class=""></div>
        <div id="divOutputAlign81" style="text-align: left" class="section36">
          <span></span><br /><span>&gt; x golden</span><br /><span
            >Useless thing that people who care about "time" and "deadlines" and whatever seem to obsess about. It's made of gold though, so it's probably worth holding on to for selling. You'll need to get out of here before you can safely fence this.</span
          ><br />
        </div>
        <div id="divOutputAlign82" style="text-align: left" class=""></div>
        <div id="divOutputAlign83" style="text-align: left" class="section37">
          <span></span><br /><span>&gt; e</span><br /><span></span><br /><span>You are in the Courtyard.</span><br /><span
            >You can see a <span id="verblink55" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace guards" data-verbs="Look at/Misdirect">palace guards</span>, a
            <span id="verblink56" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="rich man" data-verbs="Look at/Speak to/Misdirect">rich man</span> (containing a
            <span id="verblink57" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>), a
            <span id="verblink58" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace gate" data-verbs="Look at">palace gate</span> and a
            <span id="verblink59" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger pen" data-verbs="Look at">tiger pen</span> (containing a
            <span id="verblink60" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>).</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit2" data-command="go west">west</span>.</span><br /><span
            >The courtyard outside of the palace is beautifully well-kept and green with plenty of shade. The aquaducts bring water in to keep this area green, unlike the rest of the city. The trees and bushes smell crisp and clean and the warm air from the south sometimes passes through. The
            sandstone under your feet even has intricate carvings. People old, young, rich, and poor all care about this place. People usually speak in quieter voices here than the market. There are many places to sit and lounge, even some stone tables for people to gather around. There is a
            peacefulness here.</span
          ><br />
        </div>
        <div id="divOutputAlign84" style="text-align: left" class=""></div>
        <div id="divOutputAlign85" style="text-align: left" class="section38">
          <span></span><br /><span>&gt; x guards</span><br /><span
            >A pair of guards standing at the entrace to the palace. They are wearing shining, full-body plated armor that is covered in white silk cloaks with golden trim. They each have long polearms with wavy blades at the end. They must be cooking alive in that gear under the sun all day, but
            they do look pretty awesome.</span
          ><br />
        </div>
        <div id="divOutputAlign86" style="text-align: left" class=""></div>
        <div id="divOutputAlign87" style="text-align: left" class="section39">
          <span></span><br /><span>&gt; x man</span><br /><span
            >This guy is a grade-A jerk, you can tell just by how he stands there, doing nothing. He has a long, thin moustache that he is swirling in his finger as he stares into the tiger pen, mumbling something to himself. His nails are clean, hair is shiny, skin is powdered, clothes look brand
            new, and when you get close, he smells like those expensive soaps you're not even allowed near in the market. He's wearing a long robe with all sorts of fine patterns sewn in. Loosely tied to a sash on his waist is a small
            <span id="verblink61" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>.</span
          ><br />
        </div>
        <div id="divOutputAlign88" style="text-align: left" class=""></div>
        <div id="divOutputAlign89" style="text-align: left" class="section40"><span></span><br /><span>&gt; x purse</span><br /><span>A small, velvet purse with a golden trimmed clasp. You can tell there is something inside of it by how it hangs with weight.</span><br /></div>
        <div id="divOutputAlign90" style="text-align: left" class=""></div>
        <div id="divOutputAlign91" style="text-align: left" class="section41">
          <span></span><br /><span>&gt; x gate</span><br /><span>A pair of beautiful doors that lead into the palace. They are wide, tall, and made of some kind of gilded metal. You might not even be able to open them if you tried. They probably weigh more than a hippo each.</span><br />
        </div>
        <div id="divOutputAlign92" style="text-align: left" class=""></div>
        <div id="divOutputAlign93" style="text-align: left" class="section42">
          <span></span><br /><span>&gt; x pen</span><br /><span
            >A large, walled off area that is about 1 story below the ground. If you walk to the edge of the wall, you can look down inside. Inside the pen is a grassy hill and several trees, a small pond, and a little cave near the back of the hill. A thick ship-rope hangs from the tree with a
            leather ball tied to the end, dangling just above the ground. Clearly the tiger enjoys playing with it because it is covered in scratches and gouges and has a heavy patina worn in.</span
          ><br /><span>It contains a <span id="verblink62" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>.</span><br />
        </div>
        <div id="divOutputAlign94" style="text-align: left" class=""></div>
        <div id="divOutputAlign95" style="text-align: left" class="section43"><span></span><br /><span>&gt; x tiger</span><br /><span>A majestic, muscular tiger. It is currently napping on the sunny side of the hill in its pen.</span><br /></div>
        <div id="divOutputAlign96" style="text-align: left" class=""></div>
        <div id="divOutputAlign97" style="text-align: left" class="section44">
          <span></span><br /><span>&gt; w</span><br /><span></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink63" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span> (containing a
            <span id="verblink64" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pouch" data-verbs="Look at/Pick">pouch</span>), a
            <span id="verblink65" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span> (containing a
            <span id="verblink66" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pocket" data-verbs="Look at/Pick">pocket</span>), a
            <span id="verblink67" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink68" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink69" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink70" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign98" style="text-align: left" class=""></div>
        <div id="divOutputAlign99" style="text-align: left" class="section45">
          <span></span><br /><span>&gt; x poor</span><br /><span>An older, poor woman who is shuffling about in the crowd. She is probably getting into some kind of trouble, just like you. You make eye contact for a moment and she gives you a mischeivious grin with a few teeth missing.</span><br />
        </div>
        <div id="divOutputAlign100" style="text-align: left" class=""></div>
        <div id="divOutputAlign101" style="text-align: left" class="section46"><span></span><br /><span>&gt; x pouch</span><br /><span>A worn, burlap pouch. It is tied at the top using a string. It looks flat as it flops about. She is probably nearly as poor as you are.</span><br /></div>
        <div id="divOutputAlign102" style="text-align: center" class="section46">
          <span
            ><br />You take a moment and think to yourself... You haven't even tried to <span id="verblink71" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command=" look at"> look at</span> or
            <span id="verblink72" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command=" examine"> examine</span> that
            <span id="verblink73" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu" data-elementid="hairpin" data-verbs="Look at/Use/Drop">hairpin</span> you picked up. Maybe the
            <span id="verblink74" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span> carried it for a reason, other than for her hair?<br /></span
          ><br />
        </div>
        <div id="divOutputAlign103" style="text-align: left" class="section46"></div>
        <div id="divOutputAlign104" style="text-align: left" class=""></div>
        <div id="divOutputAlign105" style="text-align: left" class="section47">
          <span></span><br /><span>&gt; x hairpin</span><br /><span>A plain, thin, single-needle, bronze hairpin with a tiny flattened plate at one end. It is about the same length as your long finger.</span><br /><span>You know... this might work really well for picking locks.</span><br />
        </div>
        <div id="divOutputAlign106" style="text-align: center" class="section47">
          <span><br />You learn how to <b>PICK</b> locks using the hairpin!<br /></span><br />
        </div>
        <div id="divOutputAlign107" style="text-align: left" class="section47">
          <span
            >Try using <span id="verblink75" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pick">pick</span> on locked things to unlock them. But beware: you don't want to pick any locks while someone is looking. Make sure you're out of sight when you
            do this.</span
          ><br />
        </div>
        <div id="divOutputAlign108" style="text-align: left" class=""></div>
        <div id="divOutputAlign109" style="text-align: left" class="section48">
          <span></span><br /><span>&gt; x monkey</span><br /><span
            >A lanky monkey wearing a little purple vest. It always seems to be in the market. You figure it used to be (or still is) someone's pet, since it is so comfortable around people and has a sense of fashion. It doesn't pay any attention to you as it swings about between the
            stalltops.</span
          ><br />
        </div>
        <div id="divOutputAlign110" style="text-align: left" class=""></div>
        <div id="divOutputAlign111" style="text-align: left" class="section49"><span></span><br /><span>&gt; x pocket</span><br /><span>The vest has a visible pocket on the left side exterior.</span><br /></div>
        <div id="divOutputAlign112" style="text-align: left" class=""></div>
        <div id="divOutputAlign113" style="text-align: left" class="section50">
          <span></span><br /><span>&gt; e</span><br /><span></span><br /><span>You are in the Courtyard.</span><br /><span
            >You can see a <span id="verblink76" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace guards" data-verbs="Look at/Misdirect">palace guards</span>, a
            <span id="verblink77" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="rich man" data-verbs="Look at/Speak to/Misdirect">rich man</span> (containing a
            <span id="verblink78" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>), a
            <span id="verblink79" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace gate" data-verbs="Look at">palace gate</span> and a
            <span id="verblink80" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger pen" data-verbs="Look at">tiger pen</span> (containing a
            <span id="verblink81" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>).</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit2" data-command="go west">west</span>.</span><br /><span
            >The courtyard outside of the palace is beautifully well-kept and green with plenty of shade. The aquaducts bring water in to keep this area green, unlike the rest of the city. The trees and bushes smell crisp and clean and the warm air from the south sometimes passes through. The
            sandstone under your feet even has intricate carvings. People old, young, rich, and poor all care about this place. People usually speak in quieter voices here than the market. There are many places to sit and lounge, even some stone tables for people to gather around. There is a
            peacefulness here.</span
          ><br />
        </div>
        <div id="divOutputAlign114" style="text-align: left" class=""></div>
        <div id="divOutputAlign115" style="text-align: left" class="section51">
          <span></span><br /><span>&gt; pick purse</span><br /><span>You take some <span id="verblink82" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu" data-elementid="silver coins" data-verbs="Look at/Use/Drop">silver coins</span>. <i>Score!</i></span
          ><br /><span>The man catches you just after you swiped his coins. He yells out for the guards, pointing at you while clutching his chest dramatically with his other hand. Uh oh, time to book it out of here.</span><br />
        </div>
        <div id="divOutputAlign116" style="text-align: left" class=""></div>
        <div id="divOutputAlign117" style="text-align: left" class="section52">
          <span></span><br /><span>&gt; w</span><br /><span></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink83" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span> (containing a
            <span id="verblink84" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pouch" data-verbs="Look at/Pick">pouch</span>), a
            <span id="verblink85" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span> (containing a
            <span id="verblink86" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pocket" data-verbs="Look at/Pick">pocket</span>), a
            <span id="verblink87" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink88" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink89" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink90" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign118" style="text-align: left" class=""></div>
        <div id="divOutputAlign119" style="text-align: left" class="section53">
          <span></span><br /><span>&gt; x guard</span><br /><span
            >A fearsome, tall guard with chainmail armor and a closed-visor helmet stands about half of a block away from the bakery, looking into the market square. They're standing almost perfectly straight but you can see their eyes busily darting about. As you walk past them, you can hear the
            intensity of their breathing through their visor, like steam from a dragon's mouth. They have one hand resting on a sword's pommel, which is sheathed on their belt. You can tell by the patina on the sword handle's leather that they've seen a lot of action. This guard is not to be messed
            with.</span
          ><br />
        </div>
        <div id="divOutputAlign120" style="text-align: center" class="section53">
          <span><br />You thought you were in the clear, but the guards have caught up with you. You put your hands up as they get close. They haul you off to jail.</span><br />
        </div>
        <div id="divOutputAlign121" style="text-align: left" class="section53"></div>
        <div id="divOutputAlign122" style="text-align: center" class="section53">
          <span
            ><br />You take a moment and think to yourself... You haven't even tried to <span id="verblink91" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command=" look at"> look at</span> or
            <span id="verblink92" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command=" examine"> examine</span> that
            <span id="verblink93" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pebble" data-verbs="Look at/Use/Drop">pebble</span> you picked up. Maybe the
            <span id="verblink94" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span> carried it for a reason, other than just good luck?<br /></span
          ><br />
        </div>
        <div id="divOutputAlign123" style="text-align: left" class="section53">
          <span></span><br /><span>You are in a Jail Cell.</span><br /><span
            >You can see a <span id="verblink95" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="grate" data-verbs="Look at/Pick">grate</span>, a
            <span id="verblink96" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="jail guard" data-verbs="Look at/Speak to/Misdirect">jail guard</span> and a
            <span id="verblink97" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="chair" data-verbs="Look at">chair</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="Jail Exit" data-command="go west">west</span>.</span><br /><span
            >A dark, damp underground holding area under the palace, lit by torchlight. This is where they take the minor criminals and it's the best jail in the city. The really bad criminals go to the dungeon at the edge of town where everyone gets sick and the guards are mean. This jail exists
            because the lord set lenient laws in an attempt to distance his reputation from his deeply cruel father (the messed-up guy who ruled before him). As a result, petty theft results in a 1-day hold in the palace jail overnight instead of losing a hand by sword on the spot. You got into
            theft just in time. One generation sooner and you'd already have lost dozens of hands to the local guards. They catch you stealing bread pretty much every other day now.</span
          ><br /><span><br />The watch you were carrying has been confiscated by the guards.</span><br /><span><br />The coins you were carrying have been confiscated by the guards. They pay themselves a little bonus for their troubles.</span><br />
        </div>
        <div id="divOutputAlign124" style="text-align: left" class=""></div>
        <div id="divOutputAlign125" style="text-align: left" class="section54"><span></span><br /><span>&gt; x pebble</span><br /><span>An ordinary pebble. But you know what? It gives you an idea...</span><br /></div>
        <div id="divOutputAlign126" style="text-align: center" class="section54">
          <span><br />You learn how to <b>MISDIRECT</b>.<br /></span><br />
        </div>
        <div id="divOutputAlign127" style="text-align: left" class="section54">
          <span
            >As long as you have a pebble in your inventory, you can try to use it to distract someone. Try to <span id="verblink98" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="misdirect">misdirect</span> a target, but beware: you'll lose
            your pebble when you do and might have to find another one.</span
          ><br />
        </div>
        <div id="divOutputAlign128" style="text-align: left" class=""></div>
        <div id="divOutputAlign129" style="text-align: left" class="section55"><span></span><br /><span>&gt; pick grate</span><br /><span>No way, the guard is sitting right there! Picking the lock right now is a terrible idea.</span><br /></div>
        <div id="divOutputAlign130" style="text-align: left" class=""></div>
        <div id="divOutputAlign131" style="text-align: left" class="section56">
          <span></span><br /><span>&gt; misdirect guard</span><br /><span>You toss your pebble near them. They look at it for a second and then look back at you. "Knock it off, I'm getting to the good part in this thing."</span><br />
        </div>
        <div id="divOutputAlign132" style="text-align: center" class="section56">
          <span><br />You have lost your <b>pebble</b>. You'll need to find another one if you want to <span id="verblink99" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="misdirect">misdirect</span> again.<br /></span><br />
        </div>
        <div id="divOutputAlign133" style="text-align: left" class="section56"></div>
        <div id="divOutputAlign134" style="text-align: left" class=""></div>
        <div id="divOutputAlign135" style="text-align: left" class="section57">
          <span></span><br /><span>&gt; x guard</span><br /><span
            >A guard sits slumped in a chair, spear in one hand and a book in their other. They look bored out of their mind as they read; it must not be a very good book. Every few minutes they turn a new page by awkwardly resting their spear handle on their shoulder to free their other hand for a
            moment.</span
          ><br />
        </div>
        <div id="divOutputAlign136" style="text-align: left" class=""></div>
        <div id="divOutputAlign137" style="text-align: left" class="section58">
          <span></span><br /><span>&gt; watch</span><br /><span
            >You wait for a while, listening to the guard turn the pages in their book. Eventually they get up and wordlessly walk out of the room for the changing of the guard. Nobody comes back to take their place. It must be meal time. The silence is a bit unnerving. You're the only soul in the
            jail right now, all alone.</span
          ><br />
        </div>
        <div id="divOutputAlign138" style="text-align: left" class=""></div>
        <div id="divOutputAlign139" style="text-align: left" class="section59">
          <span></span><br /><span>&gt; pick grate</span><br /><span>You reach through the grate and find the keyhold with your hairpin. After a few minutes of fiddling with the lock, you feel the tumblers settle and you rotate the mechanism. It unlocks. You're free!</span><br />
        </div>
        <div id="divOutputAlign140" style="text-align: left" class=""></div>
        <div id="divOutputAlign141" style="text-align: left" class="section60">
          <span></span><br /><span>&gt; w</span><br /><span></span><br /><span>You are in the Palace Hall.</span><br /><span
            >You can see a <span id="verblink100" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="vizier" data-verbs="Look at/Speak to/Misdirect">vizier</span>, a
            <span id="verblink101" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="hall window" data-verbs="Look at">hall window</span> and a
            <span id="verblink102" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="door" data-verbs="Look at/Pick">door</span>.</span
          ><br /><span
            >You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit3" data-command="go west">west</span> or
            <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="Exit to Jail" data-command="go east">east</span>.</span
          ><br /><span
            >This long, empty, dimly lit hall sparkles with gold. Columns line the hallway, like immovable soldiers facing each other in silence. Mirrors are arranged along the ceiling and catch rays of pure light, but the room is so tall that where you stand is still fairly dark and shadowed. You
            can feel cool air coming from somewhere you can't see like a breeze in the night. It nearly gives you goosebumps. You've never felt cool air like that anywhere in your life, even on the coldest nights in the winter season. It feels wonderful. The hall is mostly silent and if you
            concentrate hard enough, you can hear faint scribbling sounds of a quill on parchment. At the end of the hall, past all of the columns you can make out the castle's old vizier, sitting at a desk with a candle lit, writing away. The hallway is joined by another hall at the halfway mark,
            but it is filled with patrolling guards. They seem to leave this hallway alone, for some reason. There is a single window which is across the hall from you, left open.</span
          ><br />
        </div>
        <div id="divOutputAlign142" style="text-align: left" class=""></div>
        <div id="divOutputAlign143" style="text-align: left" class="section61">
          <span></span><br /><span>&gt; x viz</span><br /><span
            >The ruler's most trusted advisor. They are ancient. You can barely make out their eyes, their wrinkles droop so far down their forehead. It's a miracle they're able to see anything at all. They seem to be busy scribbling away at some important documents.</span
          ><br />
        </div>
        <div id="divOutputAlign144" style="text-align: left" class=""></div>
        <div id="divOutputAlign145" style="text-align: left" class="section62">
          <span></span><br /><span>&gt; x hall window</span><br /><span>A window leading to the west. It is the only window in this hallway and it is left open. How convenient. Looking out, below you can see the hedge maze that used to be open to the public. It looks very unkept and messy.</span
          ><br />
        </div>
        <div id="divOutputAlign146" style="text-align: left" class=""></div>
        <div id="divOutputAlign147" style="text-align: left" class="section63"><span></span><br /><span>&gt; door</span><br /><span>I don't understand your command.</span><br /></div>
        <div id="divOutputAlign148" style="text-align: left" class=""></div>
        <div id="divOutputAlign149" style="text-align: left" class="section64">
          <span></span><br /><span>&gt; x door</span><br /><span>A plain, wooden door. It is behind the vizier's desk.</span><br /><span>It is locked with a large chain and padlock in the front. A strange way to lock a door.</span><br />
        </div>
        <div id="divOutputAlign150" style="text-align: left" class=""></div>
        <div id="divOutputAlign151" style="text-align: left" class="section65"><span></span><br /><span>&gt; e</span><br /><span>Going back to jail? Not a good idea.</span><br /></div>
        <div id="divOutputAlign152" style="text-align: left" class=""></div>
        <div id="divOutputAlign153" style="text-align: left" class="section66">
          <span></span><br /><span>&gt; w</span><br /><span>You leap out of the hall window and into an old, overgrown maze outside of the palace. After wandering through it for a little while, you find yourself crawling out of some bushes and back into the courtyard.</span><br />
        </div>
        <div id="divOutputAlign154" style="text-align: center" class="section66">
          <span><br />You have unlocked a secret path between the courtyard and the palace hall. You can use this path freely.</span><br />
        </div>
        <div id="divOutputAlign155" style="text-align: left" class="section66">
          <span></span><br /><span>You are in the Courtyard.</span><br /><span
            >You can see a <span id="verblink103" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace guards" data-verbs="Look at/Misdirect">palace guards</span>, a
            <span id="verblink104" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="rich man" data-verbs="Look at/Speak to/Misdirect">rich man</span> (containing a
            <span id="verblink105" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>), a
            <span id="verblink106" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace gate" data-verbs="Look at">palace gate</span> and a
            <span id="verblink107" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger pen" data-verbs="Look at">tiger pen</span> (containing a
            <span id="verblink108" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>).</span
          ><br /><span
            >You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit2" data-command="go west">west</span> or
            <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="old maze" data-command="go northwest">northwest</span>.</span
          ><br /><span
            >The courtyard outside of the palace is beautifully well-kept and green with plenty of shade. The aquaducts bring water in to keep this area green, unlike the rest of the city. The trees and bushes smell crisp and clean and the warm air from the south sometimes passes through. The
            sandstone under your feet even has intricate carvings. People old, young, rich, and poor all care about this place. People usually speak in quieter voices here than the market. There are many places to sit and lounge, even some stone tables for people to gather around. There is a
            peacefulness here.</span
          ><br />
        </div>
        <div id="divOutputAlign156" style="text-align: left" class=""></div>
        <div id="divOutputAlign157" style="text-align: left" class="section67">
          <span></span><br /><span>&gt; w</span><br /><span></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink109" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span> (containing a
            <span id="verblink110" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pouch" data-verbs="Look at/Pick">pouch</span>), a
            <span id="verblink111" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span> (containing a
            <span id="verblink112" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pocket" data-verbs="Look at/Pick">pocket</span>), a
            <span id="verblink113" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink114" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink115" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink116" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign158" style="text-align: left" class=""></div>
        <div id="divOutputAlign159" style="text-align: left" class="section68"><span></span><br /><span>&gt; x pocket</span><br /><span>The vest has a visible pocket on the left side exterior. It is bulging, as if totally stuffed.</span><br /></div>
        <div id="divOutputAlign160" style="text-align: left" class=""></div>
        <div id="divOutputAlign161" style="text-align: left" class="section69">
          <span></span><br /><span>&gt; pick pocket</span><br /><span>You take a <span id="verblink117" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pebble" data-verbs="Look at/Use/Drop">pebble</span>.</span><br /><span
            >You take a <span id="verblink118" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu" data-elementid="golden pocket watch" data-verbs="Look at/Use/Drop">golden pocket watch</span>. <i>Score!</i></span
          ><br />
        </div>
        <div id="divOutputAlign162" style="text-align: left" class=""></div>
        <div id="divOutputAlign163" style="text-align: left" class="section70"><span></span><br /><span>&gt; misdirect woman</span><br /><span>I doubt that would do any good...</span><br /></div>
        <div id="divOutputAlign164" style="text-align: left" class=""></div>
        <div id="divOutputAlign165" style="text-align: left" class="section71">
          <span></span><br /><span>&gt; misdirect baker</span><br /><span
            >You toss your pebble near them. They look at it for a second and then continue their work. "Annoying monkey, never leaving me alone..." they mutter under their breath. The baker is probably already distracted by their work.</span
          ><br />
        </div>
        <div id="divOutputAlign166" style="text-align: center" class="section71">
          <span><br />You have lost your <b>pebble</b>. You'll need to find another one if you want to <span id="verblink119" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="misdirect">misdirect</span> again.<br /></span><br />
        </div>
        <div id="divOutputAlign167" style="text-align: left" class="section71"></div>
        <div id="divOutputAlign168" style="text-align: left" class=""></div>
        <div id="divOutputAlign169" style="text-align: left" class="section72"><span></span><br /><span>&gt; x pocket</span><br /><span>The vest has a visible pocket on the left side exterior. It is bulging, as if totally stuffed.</span><br /></div>
        <div id="divOutputAlign170" style="text-align: left" class=""></div>
        <div id="divOutputAlign171" style="text-align: left" class="section73">
          <span></span><br /><span>&gt; pick pocket</span><br /><span>You take a <span id="verblink120" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pebble" data-verbs="Look at/Use/Drop">pebble</span>.</span><br />
        </div>
        <div id="divOutputAlign172" style="text-align: left" class=""></div>
        <div id="divOutputAlign173" style="text-align: left" class="section74"><span></span><br /><span>&gt; misdirect guard</span><br /><span>You toss your pebble near them. They look at it for a second and then look back at you. "This isn't a time for games, kid. Move along."</span><br /></div>
        <div id="divOutputAlign174" style="text-align: center" class="section74">
          <span><br />You have lost your <b>pebble</b>. You'll need to find another one if you want to <span id="verblink121" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="misdirect">misdirect</span> again.<br /></span><br />
        </div>
        <div id="divOutputAlign175" style="text-align: left" class="section74"></div>
        <div id="divOutputAlign176" style="text-align: left" class=""></div>
        <div id="divOutputAlign177" style="text-align: left" class="section75">
          <span></span><br /><span>&gt; pick pocket</span><br /><span>You take a <span id="verblink122" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pebble" data-verbs="Look at/Use/Drop">pebble</span>.</span><br />
        </div>
        <div id="divOutputAlign178" style="text-align: left" class=""></div>
        <div id="divOutputAlign179" style="text-align: left" class="section76">
          <span></span><br /><span>&gt; misdirect monkey</span><br /><span>You toss your pebble near the monkey, but its lightning-fast reflexes kick in and it catches it. It gives you a little "ooh-ooh aah-aah" and a dance, as if thanking you before putting the pebble back into their pocket.</span
          ><br />
        </div>
        <div id="divOutputAlign180" style="text-align: center" class="section76">
          <span><br />You have lost your <b>pebble</b>. You'll need to find another one if you want to <span id="verblink123" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="misdirect">misdirect</span> again.<br /></span><br />
        </div>
        <div id="divOutputAlign181" style="text-align: left" class="section76"></div>
        <div id="divOutputAlign182" style="text-align: left" class=""></div>
        <div id="divOutputAlign183" style="text-align: left" class="section77">
          <span></span><br /><span>&gt; pick pocket</span><br /><span>You take a <span id="verblink124" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pebble" data-verbs="Look at/Use/Drop">pebble</span>.</span><br />
        </div>
        <div id="divOutputAlign184" style="text-align: left" class=""></div>
        <div id="divOutputAlign185" style="text-align: left" class="section78"><span></span><br /><span>&gt; x pocket</span><br /><span>The vest has a visible pocket on the left side exterior.</span><br /></div>
        <div id="divOutputAlign186" style="text-align: left" class=""></div>
        <div id="divOutputAlign187" style="text-align: left" class="section79">
          <span></span><br /><span>&gt; e</span><br /><span></span><br /><span>You are in the Courtyard.</span><br /><span
            >You can see a <span id="verblink125" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace guards" data-verbs="Look at/Misdirect">palace guards</span>, a
            <span id="verblink126" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="rich man" data-verbs="Look at/Speak to/Misdirect">rich man</span> (containing a
            <span id="verblink127" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>), a
            <span id="verblink128" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace gate" data-verbs="Look at">palace gate</span> and a
            <span id="verblink129" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger pen" data-verbs="Look at">tiger pen</span> (containing a
            <span id="verblink130" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>).</span
          ><br /><span
            >You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit2" data-command="go west">west</span> or
            <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="old maze" data-command="go northwest">northwest</span>.</span
          ><br /><span
            >The courtyard outside of the palace is beautifully well-kept and green with plenty of shade. The aquaducts bring water in to keep this area green, unlike the rest of the city. The trees and bushes smell crisp and clean and the warm air from the south sometimes passes through. The
            sandstone under your feet even has intricate carvings. People old, young, rich, and poor all care about this place. People usually speak in quieter voices here than the market. There are many places to sit and lounge, even some stone tables for people to gather around. There is a
            peacefulness here.</span
          ><br />
        </div>
        <div id="divOutputAlign188" style="text-align: left" class=""></div>
        <div id="divOutputAlign189" style="text-align: left" class="section80"><span></span><br /><span>&gt; misdirect tiger</span><br /><span>You toss your pebble near them. They lazily open an eye and bat it away with their paw. They go back to napping.</span><br /></div>
        <div id="divOutputAlign190" style="text-align: center" class="section80">
          <span><br />You have lost your <b>pebble</b>. You'll need to find another one if you want to <span id="verblink131" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="misdirect">misdirect</span> again.<br /></span><br />
        </div>
        <div id="divOutputAlign191" style="text-align: left" class="section80"></div>
        <div id="divOutputAlign192" style="text-align: left" class=""></div>
        <div id="divOutputAlign193" style="text-align: left" class="section81">
          <span></span><br /><span>&gt; w</span><br /><span></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink132" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span> (containing a
            <span id="verblink133" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pouch" data-verbs="Look at/Pick">pouch</span>), a
            <span id="verblink134" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span> (containing a
            <span id="verblink135" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pocket" data-verbs="Look at/Pick">pocket</span>), a
            <span id="verblink136" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink137" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink138" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink139" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign194" style="text-align: left" class=""></div>
        <div id="divOutputAlign195" style="text-align: left" class="section82">
          <span></span><br /><span>&gt; pick pocket</span><br /><span>You take a <span id="verblink140" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pebble" data-verbs="Look at/Use/Drop">pebble</span>.</span><br />
        </div>
        <div id="divOutputAlign196" style="text-align: left" class=""></div>
        <div id="divOutputAlign197" style="text-align: left" class="section83"><span></span><br /><span>&gt; r</span><br /><span>I don't understand your command.</span><br /></div>
        <div id="divOutputAlign198" style="text-align: left" class=""></div>
        <div id="divOutputAlign199" style="text-align: left" class="section84">
          <span></span><br /><span>&gt; e</span><br /><span></span><br /><span>You are in the Courtyard.</span><br /><span
            >You can see a <span id="verblink141" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace guards" data-verbs="Look at/Misdirect">palace guards</span>, a
            <span id="verblink142" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="rich man" data-verbs="Look at/Speak to/Misdirect">rich man</span> (containing a
            <span id="verblink143" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>), a
            <span id="verblink144" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace gate" data-verbs="Look at">palace gate</span> and a
            <span id="verblink145" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger pen" data-verbs="Look at">tiger pen</span> (containing a
            <span id="verblink146" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>).</span
          ><br /><span
            >You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit2" data-command="go west">west</span> or
            <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="old maze" data-command="go northwest">northwest</span>.</span
          ><br /><span
            >The courtyard outside of the palace is beautifully well-kept and green with plenty of shade. The aquaducts bring water in to keep this area green, unlike the rest of the city. The trees and bushes smell crisp and clean and the warm air from the south sometimes passes through. The
            sandstone under your feet even has intricate carvings. People old, young, rich, and poor all care about this place. People usually speak in quieter voices here than the market. There are many places to sit and lounge, even some stone tables for people to gather around. There is a
            peacefulness here.</span
          ><br />
        </div>
        <div id="divOutputAlign200" style="text-align: left" class=""></div>
        <div id="divOutputAlign201" style="text-align: left" class="section85"><span></span><br /><span>&gt; misdirect guards</span><br /><span>You toss your pebble near them. They look at it for a second and then look back at you. "This isn't a time for games, kid. Move along."</span><br /></div>
        <div id="divOutputAlign202" style="text-align: center" class="section85">
          <span><br />You have lost your <b>pebble</b>. You'll need to find another one if you want to <span id="verblink147" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="misdirect">misdirect</span> again.<br /></span><br />
        </div>
        <div id="divOutputAlign203" style="text-align: left" class="section85"></div>
        <div id="divOutputAlign204" style="text-align: left" class=""></div>
        <div id="divOutputAlign205" style="text-align: left" class="section86">
          <span></span><br /><span>&gt; w</span><br /><span></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink148" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span> (containing a
            <span id="verblink149" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pouch" data-verbs="Look at/Pick">pouch</span>), a
            <span id="verblink150" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span> (containing a
            <span id="verblink151" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pocket" data-verbs="Look at/Pick">pocket</span>), a
            <span id="verblink152" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink153" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink154" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink155" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign206" style="text-align: left" class=""></div>
        <div id="divOutputAlign207" style="text-align: left" class="section87">
          <span></span><br /><span>&gt; pick pocket</span><br /><span>You take a <span id="verblink156" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pebble" data-verbs="Look at/Use/Drop">pebble</span>.</span><br />
        </div>
        <div id="divOutputAlign208" style="text-align: left" class=""></div>
        <div id="divOutputAlign209" style="text-align: left" class="section88">
          <span></span><br /><span>&gt; e</span><br /><span></span><br /><span>You are in the Courtyard.</span><br /><span
            >You can see a <span id="verblink157" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace guards" data-verbs="Look at/Misdirect">palace guards</span>, a
            <span id="verblink158" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="rich man" data-verbs="Look at/Speak to/Misdirect">rich man</span> (containing a
            <span id="verblink159" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>), a
            <span id="verblink160" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace gate" data-verbs="Look at">palace gate</span> and a
            <span id="verblink161" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger pen" data-verbs="Look at">tiger pen</span> (containing a
            <span id="verblink162" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>).</span
          ><br /><span
            >You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit2" data-command="go west">west</span> or
            <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="old maze" data-command="go northwest">northwest</span>.</span
          ><br /><span
            >The courtyard outside of the palace is beautifully well-kept and green with plenty of shade. The aquaducts bring water in to keep this area green, unlike the rest of the city. The trees and bushes smell crisp and clean and the warm air from the south sometimes passes through. The
            sandstone under your feet even has intricate carvings. People old, young, rich, and poor all care about this place. People usually speak in quieter voices here than the market. There are many places to sit and lounge, even some stone tables for people to gather around. There is a
            peacefulness here.</span
          ><br />
        </div>
        <div id="divOutputAlign210" style="text-align: left" class=""></div>
        <div id="divOutputAlign211" style="text-align: left" class="section89">
          <span></span><br /><span>&gt; misdirect man</span><br /><span>You toss your pebble deftly at a lemon fruit hanging above the rich man. The lemon falls onto his head, and in his confusion he turns around, looking up. "What was that?"</span><br />
        </div>
        <div id="divOutputAlign212" style="text-align: center" class="section89">
          <span><br />You have lost your <b>pebble</b>. You'll need to find another one if you want to <span id="verblink163" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="misdirect">misdirect</span> again.</span><br />
        </div>
        <div id="divOutputAlign213" style="text-align: left" class="section89"></div>
        <div id="divOutputAlign214" style="text-align: center" class="section89">
          <span><br />The rich man is currently distracted. Act quickly, before he catches on.</span><br />
        </div>
        <div id="divOutputAlign215" style="text-align: left" class="section89"></div>
        <div id="divOutputAlign216" style="text-align: left" class=""></div>
        <div id="divOutputAlign217" style="text-align: left" class="section90">
          <span></span><br /><span>&gt; pick purse</span><br /><span>You take some <span id="verblink164" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu" data-elementid="silver coins" data-verbs="Look at/Use/Drop">silver coins</span>. <i>Score!</i></span
          ><br /><span>He gathers himself and mutters, "not the first time I've had fruit fall on me while I'm watching the tiger..."</span><br />
        </div>
        <div id="divOutputAlign218" style="text-align: center" class="section90">
          <span><br />The rich man is no longer distracted.<br /></span><br />
        </div>
        <div id="divOutputAlign219" style="text-align: left" class="section90"></div>
        <div id="divOutputAlign220" style="text-align: left" class=""></div>
        <div id="divOutputAlign221" style="text-align: left" class="section91">
          <span></span><br /><span>&gt; w</span><br /><span></span><br /><span>You are in the Market.</span><br /><span
            >You can see a <span id="verblink165" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="poor woman" data-verbs="Look at/Speak to/Misdirect">poor woman</span> (containing a
            <span id="verblink166" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pouch" data-verbs="Look at/Pick">pouch</span>), a
            <span id="verblink167" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="monkey" data-verbs="Look at/Misdirect">monkey</span> (containing a
            <span id="verblink168" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pocket" data-verbs="Look at/Pick">pocket</span>), a
            <span id="verblink169" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="bakery stall" data-verbs="Look at">bakery stall</span> (containing a
            <span id="verblink170" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baguette" data-verbs="Look at/Take/Buy">baguette</span> and a
            <span id="verblink171" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="baker" data-verbs="Look at/Speak to/Misdirect">baker</span>) and a
            <span id="verblink172" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="market guard" data-verbs="Look at/Speak to/Misdirect">market guard</span>.</span
          ><br /><span>You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit1" data-command="go east">east</span>.</span><br /><span
            >It is bustling with people coming and going. The market stretches for city blocks in all directions, it's the heart of this city. Aside from the hole in a wall where you sleep at night, this is one of the only places where you get a sense of comfort. You love the sounds of people
            bartering, folks barking their wares, criers shouting news and the smells of purfumes, fresh oranges and lemons, and of course, all of the food being grilled, fried, and baked.</span
          ><br />
        </div>
        <div id="divOutputAlign222" style="text-align: left" class=""></div>
        <div id="divOutputAlign223" style="text-align: left" class="section92">
          <span></span><br /><span>&gt; pick pocket</span><br /><span>You take a <span id="verblink173" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="pebble" data-verbs="Look at/Use/Drop">pebble</span>.</span><br />
        </div>
        <div id="divOutputAlign224" style="text-align: left" class=""></div>
        <div id="divOutputAlign225" style="text-align: left" class="section93">
          <span></span><br /><span>&gt; e</span><br /><span></span><br /><span>You are in the Courtyard.</span><br /><span
            >You can see a <span id="verblink174" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace guards" data-verbs="Look at/Misdirect">palace guards</span>, a
            <span id="verblink175" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="rich man" data-verbs="Look at/Speak to/Misdirect">rich man</span> (containing a
            <span id="verblink176" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="purse" data-verbs="Look at/Take/Pick">purse</span>), a
            <span id="verblink177" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="palace gate" data-verbs="Look at">palace gate</span> and a
            <span id="verblink178" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger pen" data-verbs="Look at">tiger pen</span> (containing a
            <span id="verblink179" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="tiger" data-verbs="Look at/Speak to/Misdirect">tiger</span>).</span
          ><br /><span
            >You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit2" data-command="go west">west</span> or
            <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="old maze" data-command="go northwest">northwest</span>.</span
          ><br /><span
            >The courtyard outside of the palace is beautifully well-kept and green with plenty of shade. The aquaducts bring water in to keep this area green, unlike the rest of the city. The trees and bushes smell crisp and clean and the warm air from the south sometimes passes through. The
            sandstone under your feet even has intricate carvings. People old, young, rich, and poor all care about this place. People usually speak in quieter voices here than the market. There are many places to sit and lounge, even some stone tables for people to gather around. There is a
            peacefulness here.</span
          ><br />
        </div>
        <div id="divOutputAlign226" style="text-align: left" class=""></div>
        <div id="divOutputAlign227" style="text-align: left" class="section94"><span></span><br /><span>&gt; watch</span><br /><span>You wait and relax for a while in the shade of some large palms, watching the tiger continue to nap. No new opportunities present themselves.</span><br /></div>
        <div id="divOutputAlign228" style="text-align: left" class=""></div>
        <div id="divOutputAlign229" style="text-align: left" class="section95">
          <span></span><br /><span>&gt; nw</span><br /><span></span><br /><span>You are in the Palace Hall.</span><br /><span
            >You can see a <span id="verblink180" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="vizier" data-verbs="Look at/Speak to/Misdirect">vizier</span>, a
            <span id="verblink181" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="hall window" data-verbs="Look at">hall window</span> and a
            <span id="verblink182" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="door" data-verbs="Look at/Pick">door</span>.</span
          ><br /><span
            >You can go <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="exit3" data-command="go west">west</span> or
            <span style="font-weight: bold; color: #00855d" class="cmdlink exitlink disabled" data-elementid="Exit to Jail" data-command="go east">east</span>.</span
          ><br /><span
            >This long, empty, dimly lit hall sparkles with gold. Columns line the hallway, like immovable soldiers facing each other in silence. Mirrors are arranged along the ceiling and catch rays of pure light, but the room is so tall that where you stand is still fairly dark and shadowed. You
            can feel cool air coming from somewhere you can't see like a breeze in the night. It nearly gives you goosebumps. You've never felt cool air like that anywhere in your life, even on the coldest nights in the winter season. It feels wonderful. The hall is mostly silent and if you
            concentrate hard enough, you can hear faint scribbling sounds of a quill on parchment. At the end of the hall, past all of the columns you can make out the castle's old vizier, sitting at a desk with a candle lit, writing away. The hallway is joined by another hall at the halfway mark,
            but it is filled with patrolling guards. They seem to leave this hallway alone, for some reason. There is a single window which is across the hall from you, left open.</span
          ><br />
        </div>
        <div id="divOutputAlign230" style="text-align: left" class=""></div>
        <div id="divOutputAlign231" style="text-align: left" class="section96">
          <span></span><br /><span>&gt; misdirect vizier</span><br /><span
            >You sneak your way closer to the vizier while remaining hidden. You toss your pebble behind the vizier and it clatters against some metallic sounding object. The vizier suddenly jumps, their wrinkles lifting up to show wide eyes. "Oh my... what was that? Did I drop something?" They
            stand up slowly, shaking a little. "Oh my bones..." They wince. They turn around and slowly lean over. "What was that now? Hmm..."</span
          ><br />
        </div>
        <div id="divOutputAlign232" style="text-align: center" class="section96">
          <span><br />You have lost your <b>pebble</b>. You'll need to find another one if you want to <span id="verblink183" style="font-weight: bold; color: #00855d" class="cmdlink commandlink" data-elementid="" data-command="misdirect">misdirect</span> again.</span><br />
        </div>
        <div id="divOutputAlign233" style="text-align: left" class="section96"></div>
        <div id="divOutputAlign234" style="text-align: center" class="section96">
          <span><br />The vizier is currently distracted. Act quickly, before they catch on.</span><br />
        </div>
        <div id="divOutputAlign235" style="text-align: left" class="section96"></div>
        <div id="divOutputAlign236" style="text-align: left" class=""></div>
        <div id="divOutputAlign237" style="text-align: left" class="section97">
          <span></span><br /><span>&gt; pick door</span><br /><span>You swiftly move to the padlock on the door and jam your hairpin into the keyhole. You fiddle quickly, and as quietly as you can, and luckily it pops open almost right away. You're a natural at this!</span><br /><span
            >You quietly set the chain and open padlock aside and head into the room.</span
          ><br /><span></span><br /><span>You are in the Vizier's Room.</span><br /><span
            >You can see a <span id="verblink184" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="window" data-verbs="Look at/open">window</span>, a
            <span id="verblink185" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="strange equipment" data-verbs="Look at">strange equipment</span> and a
            <span id="verblink186" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu disabled" data-elementid="desk" data-verbs="Look at">desk</span>.</span
          ><br /><span
            >You walk into the room and quickly wedge a chair against the door handle so that nobody can follow you in. You won't be able to go back the way you came unless you want to spend more time in the slammer. You take a minute to let the adrenaline settle. "I'm not half bad at this thieving
            business," you think to yourself.</span
          ><br />
        </div>
        <div id="divOutputAlign238" style="text-align: left" class=""></div>
        <div id="divOutputAlign239" style="text-align: left" class="section98">
          <span></span><br /><span>&gt; x window</span><br /><span>A window leading out of the vizier's room. It's pretty high up, you probably won't be able to come back this way. You can see a wide, open, sandy valley below. It is closed.</span><br />
        </div>
        <div id="divOutputAlign240" style="text-align: left" class=""></div>
        <div id="divOutputAlign241" style="text-align: left" class="section99">
          <span></span><br /><span>&gt; x strange</span><br /><span>Strange glass baubles and glasses and vials are brewing liquids of all sorts of colors. These devices are completely unknown to you. Is this for some special kind of baking or brewing?</span><br />
        </div>
        <div id="divOutputAlign242" style="text-align: left" class=""></div>
        <div id="divOutputAlign243" style="text-align: left" class="section100">
          <span></span><br /><span>&gt; x desk</span><br /><span>A heavy, old mahogany desk. It is covered in now-hardened, once-melted wax from many years of burning candles. There are ink stains and stacks and stacks of parchment and scrolls all over.</span><br /><span
            >Hidden under piles of parchment scraps are <span id="verblink187" style="font-weight: bold; color: #00855d" class="cmdlink elementmenu" data-elementid="jewels" data-verbs="Look at/Use/Drop">jewels</span>.</span
          ><br />
        </div>
        <div id="divOutputAlign244" style="text-align: left" class=""></div>
        <div id="divOutputAlign245" style="text-align: left" class="section101">
          <span></span><br /><span>&gt; x jewels</span><br /><span
            >A small pile of shimmering little jewels, most just large enough to be set into a ring or earring. They're all kinds of blue, red, yellow, green, and white and cut into all kinds of beautiful shapes. These must be worth a fortune.</span
          ><br />
        </div>
        <div id="divOutputAlign246" style="text-align: left" class=""></div>
        <div id="divOutputAlign247" style="text-align: left" class="section102"><span></span><br /><span>&gt; take jewels</span><br /><span>You pick it up.</span><br /></div>
        <div id="divOutputAlign248" style="text-align: left" class=""></div>
        <div id="divOutputAlign249" style="text-align: left" class="section103"><span></span><br /><span>&gt; north</span><br /><span>You can't go there.</span><br /></div>
        <div id="divOutputAlign250" style="text-align: left" class=""></div>
        <div id="divOutputAlign251" style="text-align: left" class="section104"><span></span><br /><span>&gt; open window</span><br /><span>You open the window and a warm breeze greets your face. You look down to the valley below you. It's quite a long jump down...</span><br /></div>
        <div id="divOutputAlign252" style="text-align: center" class="section104">
          <span><br />You have opened the exit that leads <b>north</b> to the free valley.</span><br />
        </div>
        <div id="divOutputAlign253" style="text-align: left" class="section104"></div>
        <div id="divOutputAlign254" style="text-align: left" class=""></div>
        <div id="divOutputAlign255" style="text-align: left" class="section105">
          <span></span><br /><span>&gt; north</span><br /><span>You leap from the window to the sandy valley below.</span><br /><span></span><br /><span>You are in a Valley.</span><br /><span
            >The valley of freedom! You've done it. Nothing stands between you and the open sands. You heard if you travel further north, there is a port town. That should be a great place to fence your goods and set sail to new horizons.</span
          ><br /><span><br /><i>Calculating final score:</i></span
          ><br /><span>Your pocket lint is worth +0 score.</span><br /><span>Your silver coins are worth +1 score.</span><br /><span>Your golden pocket watch is worth +1 score.</span><br /><span>Your jewels are worth +8 score.</span><br />
        </div>
        <div id="divOutputAlign256" style="text-align: center" class="section105">
          <span><br /><b>Final score: 10/10</b></span
          ><br />
        </div>
        <div id="divOutputAlign257" style="text-align: left" class="section105"></div>
      </div>
      <div id="gamePanesFinished" style="display: block">
        <h3>Game Over</h3>
        <p>This game has finished.</p>
      </div>
    </div>
</details>

## Changes made since our play-test

**Fixes**:

<ul>
    <li>Tiger now appears in courtyard</li>
    <li>Secret path is fixed (it can be reused)</li>
    <li>Jail won't let you back in unless you get in trouble again</li>
    <li>Pebble correctly returns to monkey's pocket</li>
    <li>Removed the "take" command from the verb list for the bakery stall</li>
    <li>Fixed bug where jail guard returns too late to be included in room description</li>
    <li>Misc. typos fixed</li>
</ul>

**Improvements**:

<ul>
    <li>Score visibly increases when you acquire watch and/or coins</li>
    <li>Score visibly decreases when your loot is confiscated</li>
    <li>Clarify what "north" is in the vizier's room</li>
    <li>Added window-opening mechanic to vizier's room, to prompt player that they cannot return once they leave</li>
    <li>Add robust handling for failures (and humorous uses of) the misdirect command</li>
    <li>Added turn timers (15-turn and 20-turn) to the hairpin and pebble, respectively, if player doesn't examine or look at them (to help them get unstuck)</li>
    <li>Add better wording/hints when new objects are added to the scene</li>
    <li>Notify player more clearly when you lose your pebble</li>
    <li>Add hints for where to get new pebbles</li>
    <li>Improved line spacing for special events (to make them easier to notice)</li>
    <li>Added more dynamic descriptions that change based on object interaction state (such as empty pockets after picking, etc)</li>
</ul>
