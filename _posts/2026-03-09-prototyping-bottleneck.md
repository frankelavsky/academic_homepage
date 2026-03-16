---
layout: post
title: "On genAI: Was prototyping really a bottleneck?"
slug: prototyping-bottleneck
tags:
- prototyping
- design
- software
- llms
- large-language models
- ai
- agentic models
description: "I keep hearing folks claim that the fact we can 'prototype' so quickly now is a good thing (thanks to modern genAI). But what if the slow parts about prototyping are actually what make it worth doing?"
---

(This post is a part of my new mantra moving to Cal Poly SLO: "move SLO and repair things," which is in direct tension with the mantra from the tech industry "move fast and break things" as well as a play on the abbreviation of San Luis Obispo, where I will soon work. I want to cultivate a research culture and lifestyle focused on maintenance, careful deliberation, and *care*, as defined in the feminist sense of the word.)

<hr>
<br>

Ever since ChatGPT, folks have frequently remarked something along the lines of, "LLMs are so fast, now we can easily scaffold prototypes! Finally, the bottleneck is gone!" *Bottleneck?* Was the problem with prototyping the fact it took too long? Some nerd (Microsoft guy maybe?) said the even-more-ridiculous "finally the bottleneck from typing is gone" as if the speed of typing is what was holding back new ideas and features and improvement and so on.

<blockquote class="warning">
    <p>⚠ <b>Warning</b>:</p>
    <p>This blog post is a response to a post on LinkedIn. The original may someday be lost in time! For now, the <a href="https://www.linkedin.com/posts/ebertini_i-am-convinced-we-are-in-a-new-era-for-visual-share-7436798122770653184-CZpP?utm_source=share&utm_medium=member_desktop&rcm=ACoAADDAwBkBOdoW11I9B5DHy57VfR5jIs33Kq0">post is here, by Enrico Bertini</a>.</p>
</blockquote>

Enrico writes,

> "I am convinced we are in a new era for Visual Analytics (VA) (i.e., visual interactive data interfaces), but I am not sure we have yet realized it.
> 
> In VA, building and refining a prototype has always been a costly bottleneck. This is no longer true. A single skilled person can build a working prototype in a matter of hours. They can also thrash it and rebuild it within hours. Heck! They can even build three alternatives and show all of them in maybe 1-2 days. This is no small change. It's massive.
> 
> How do we deal with that?
> 
> All of a sudden, an idea in my head can be transformed into a tangible prototype very quickly. This has enormous implications for applied research. If I work with a partner in a specific domain, I can quickly show something rather than talk. If I am good enough, I can even build something they can use pretty quickly."

I don't want to interpret Enrico's words too harshly or in an ungenerous way (but I could, if this was all I saw!). I think Enrico has remarked in the past on many occasions that genAI is creating new challenges. And I want to unpack some assumptions I see here in this post, as well as assumptions (and dangerous ones!) that I've seen many other people express.

One of the main challenges, before I really jump in, is that building something quickly can be good *if you know exactly what you are doing*. And this is the danger! Students haven't learned all kinds of things about software and how to think about users, human cognition and perception, and more. And non-technologists are often unopinionated about the detailed design and engineering intricacies that someone who is more-experienced in technology comes to consider.

**But people tend to assume that the ideas they have in their head are really good, if they aren't used to rigorously iterating on ideas.**

Sometimes... slowing down is good for *you*, the builder! And sometimes going fast is awesome, but you must absolutely know what you're doing. (And at that point, genAI is very-rarely much of a speed-boosting tool. GenAI users tend to spend far more time checking output and logic [compared to when they write code themselves](https://arxiv.org/abs/2507.09089).)

*So, consider this blog post a response to the least-generous interpretation that one might have of the world around us; peering at the worst-case scenario uses of genAI and not just the optimistic ones.*

<hr>
<br>

<figure style="display: block; width: 90%; margin-left: auto; margin-right: auto;">
    <img src="https://www.frank.computer/images/slopzone.png" alt="The prototype slop zone by Frank Elavsky. Diagram. There are two axes. X axis is how technically refined an artifact is, starting low and increasing. Y axis is how intellectually refined an idea is, starting low and increasing. In the upper left (high idea refinement, low artifact refinement), an annotation says, 💡 what users want gnAI for (for their brilliant ideas), an arrow points to an area labeled (zone of missing skills). The in the bottom right an annotation says what genAI enables 🫠. Low fidelity prototypes fill the left side near the bottom (low technical refinement and ideation), mid-fidelity in the middle of the diagram, and high fidelity fills the upper right (high ideation, high technical refinement). A tiny slice in the top right corner (maxed on both axes) says no longer a prototype."/>
    <figcaption><i>Artifact refinement versus idea refinement, and how prototyping fits in to the picture.</i> If you believe that prototypes are merely an idea made manifest, rather than prototypes representing a means to refine the ideas they represent, this diagram might help you realize a few things. (Namely that folks often assume what they lack are skills, when they often lack skills AND well-refined ideas...)</figcaption>
</figure>

## Is iterative ideation itself a bottleneck?

In some contexts, slow prototyping is probably a "bottleneck," sure. But prototyping is central to generating an understanding of the thing you're making, questioning your assumptions, and trying to communicate the rawest components of your ideas. None of those inherently get better if you do them faster.

In terms of prototype "fidelity" (understood as "[faithfulness](https://www.frank.computer/blog/2024/01/what-is-a-prototype.html)") I reckon we need to now consider: *whose* ideas is this prototype faithful to? Is this prototype faithful to the original human creator, or are there embedded biases in this prototype's function and construction because it was made using agentic tools/modern models?

An "unfaithful" prototype now has a new meaning, because we can more easily create prototypes that *appear* to be high fidelity, but may not actually be *faithful* to the intricacies of any particular idea at all.

This line below, in particular, I think *does* have enormous implications for applied research, but I wouldn't necessarily assume that the implications are all good:

> All of a sudden, an idea in my head can be transformed into a tangible prototype very quickly. This has enormous implications for applied research.

I agree that a shift is taking place. But I don't think we should just move forward as if the act of slowly prototyping itself was a problem to solve. I would argue that the act of prototyping (*especially* when done slowly) is still valuable as a necessary step we take as creators, attempting to make something new. (As a note, I get disappointed with the view that a "prototype" is the same as "a first attempt to create something" and not "an artifact I use to reflexively to discover+congeal my own ideas and communicate with.")

## Is faster communication... *better*?

I've written about prototypes before, and what I think much of our literature misses on the subject: that prototypes are actually a tool for *communicating*. ([This blog post of mine on prototyping](https://www.frank.computer/blog/2024/01/what-is-a-prototype.html) was my most-visited post, before [my post on AI + Tools](https://www.frank.computer/blog/2025/05/just-a-tool.html) came out. Funnily enough, *this* post I'm writing right now seems to be marrying the two.)

The fact that we can communicate *faster* isn't necessarily good, if we don't have a firm grasp of the idea itself in our head in the first place. One of the best parts about prototyping, to me, are the slowest parts: you draw something out with a pencil and paper, you cut out pieces of cardboard, you use some lego bricks to scaffold something, you get up to a whiteboard with a few other people and start squeaking your pens across the blank canvas together... *and you talk about that stuff with each other.* I am in love with the feeling of new thoughts forming in my head. A thought coming into being? Boring. But an existing thought refining and honing and strengthening? It's beautiful.

"Prototyping" is *not* a linear pipeline that goes from an idea in your head into a material artifact that represents that idea.

**Prototyping is a method of symbol-making. And we use those symbols to communicate ideas.**

And this is why I am actually worried about prototyping that moves *too* fast. And in fact fast-prototyping-as-a-problem isn't new! Researchers who studied "fidelity" in prototyping have long discussed how moving too quickly to higher fidelity prototyping can bias your future ideas, bias your outcomes, and ultimately produce *more* costs, not less, down the road (see this [seminal summary of the great older battles on fidelity by Rudd, Stern, and Isensee](https://dl.acm.org/doi/pdf/10.1145/223500.223514)).

## Are genAI prototypes *anti-social*?

So back to Enrico's argument here... I'm not sold that faster = better and *certainly* not sold that faster = better = cheaper (specifically responding to the sentiment in his post that it has "always been a costly bottleneck"). I think that existing literature would argue quite the opposite. To me, there are three dangers with going *too* fast: Faster = 1) more assumptions are missed in the core ideas because you have less time to validate and test fundamental bias, 2) ideas that appear already-refined become immune to questioning because they appear to be already-solved problems, and 3) less time spent socially co-constructing.

*Yes!* You heard me: Faster prototypes can become *anti-social* prototypes. This final point (which I am making, not necessarily something I've read in the literature on this) is actually the most important one to make: **prototypes are about symbol-making for the purpose of communicating**. Forming an idea *with others* is oe of my favorite activities on this earth. We're making meaning together! How beautiful is that? Not only do we create things together, but through the process of co-creating meaning, I find myself. I gain a sense of individual *and* collective identity through co-creation.

I don't just order a meal and a chef prepares it (which is the genAI design model: you, the customer, and the model, the service). Instead, I learn that I, myself, by taking action to sate my hunger can become a *chef-in-training*. By learning new ingredients, by learning how to operate tools, and through trial and error... I can gain a sense of identity beyond the customer-consumer that genAI companies want me to imagine for myself. And the best part of the self-discovery process? My partners become my line cooks, sous chef, wait staff and so on. We form a team around this new idea we create together. *Why would I ever want a machine learning model to replace the social aspects of making?* The greatest privilege of creation is finding yourself in the people you co-create with.

But even selfishly: If you were the only person left alive on this earth, yet you still learned how to speak, you would likely not lose your internal dialogue. You would still speak, even to yourself, to think through things. And prototyping, as an act and process (not a destination), is about that symbol-making. You're working through whatever idea needs forming and needs new symbols for expressing. Prototypes are a form of self-socializing ideation. And their inherently symbol-rich, generative nature makes them ideal for socializing with others.

Enrico acknowledges the power of socializing in his post:

> "If I work with a partner in a specific domain, I can quickly show something rather than talk. If I am good enough, I can even build something they can use pretty quickly."

And here is the danger: sharing something with others that is *too polished* is exactly what existing literature on prototyping warns about! You're sharing an over-developed set of assumptions! People mostly give feedback on little cosmetic details once you show them something pretty far along. And this behavioral barrier can be overcome with a good conversation partner (who might understand that what you are showing them is potentially throw-away), but this is unsupported by current literature that observes how people interact with prototypes (that generally people, if unprompted, will give less fundamental, high-level critique and engagement if the prototype is more-polished).

Inviting someone to write a language with you is different than asking someone to critique a sentence you wrote. What you want, when socializing a prototype, are conversation partners who want to question your core assumptions about whatever problems you believe exist and are trying to solve. Prototyping that is low fidelity (and slower) invites this language-crafting level of engagement with peers. Higher fidelity (with LLM assistance or otherwise) invites a copyediting level of feedback. We *want* socialization on the core symbols and ideas we choose to construct! And that might always have a *human* bottleneck built into it (for as long as we humans are in charge of prototyping, that is).

## Socially constructing meaning is slow (and good!)

But just to drive this home: ***socializing your idea* is the real value of a prototype**. Socializing a raw idea is a fundamental epistemic activity that we do. The philosohpical existentialists and absurdists spoke to this: existence precedes essence. *We* give the world around us essence. *We*, the collective subject that is humanity, assign meaning to the world. Prototyping is a radical, social act of communal meaning-making.

And I honestly wouldn't like ideation, as this quintessentially human act, if I only ever did it alone or with a machine that simply confirms my biases and listens to my instructions. Refining, discussing, sharing, mixing, appropriating, and fusing ideas are actions that really only come into the picture once we have a prototype in between a few people who are trying to figure something out together.

But *why* is socializing so important? Because our intelligence is *positional* and *situated*. We have "horizons" of knowledge, and limits, as singular beings. We are not objective. Yet through social inclusion in the act of making and forming ideas, we broaden the angles and horizons of our social constructs. And for this reason, prototypes that are socialized are simply better, more meaningful creations. I'd even argue that a prototype that isn't socialized isn't a prototype at all, it is just an early attempt at making something: the focus is on the *object* being made, not the idea it represents. And it's that human socialization and collective meaning-making that turn an artifact-in-process into a prototype that is refining something outside of itself: an *idea-in-process*.

In "[what do prototypes prototype?](https://hci.stanford.edu/courses/cs247/2012/readings/WhatDoPrototypesPrototype.pdf)", Houde and Hill argue that the separation of artifact and idea is key to understanding the value of prototyping: the prototype isn't the idea itself, it is just a symbol of the idea (hence, why I write about why fidelity = faithfulness and not something like "quality").

I worry about prototypes that are *too* refined *too* soon. Will they alienate our ideas, because our ideas are less inviting for critique/reshaping at fundamental levels? (Isn't it ironic, that using a *language model* possibly holds us back from building a truly social new set of symbols for communicating an emerging, shared space of thinking?)

A good prototype can be made quickly, but it *needs* to be a little bit shitty, too; it's basically a requirement. And in terms of pure speed, the fastest prototypes I've ever built are still far faster than an LLM-prompted mini-app and contain far fewer baked in patterns and assumptions about what I'm trying to accomplish. The humble pen and paper, cut out pieces of paper, and lego brick styles of prototyping are all undefeated ways to build a shared set of symbols about a new idea with someone. Plus, they're fun to collaborate with, as a design material! Until we can have easy to use, small, modular, generic, programmable soft and hard materials, doing things with smoke and mirrors and little trinkets is still my favorite way to do things.

Anyway, this blog post is a largely-unstructured brain-dump in response to a linkedin post. Thanks to Enrico for posting it! It certainly got my juices flowing.

And it *does* seem ironic to me to socialize the idea that prototyping=faster=cheaper=good (that all of these things are true and related). That seems like an idea that has been developed *too far*... it has too much fidelity, not enough prototyping. Perhaps I would recommend going back to the drawing board and re-assessing this?

<hr>
<br>

## Bonus take: the psychology of *faster = better*

Now, the real spicy take of mine (imagine the armchair psychologist within me saying this): I don't think the "bottleneck" that existed was any more than simply manufactured *human impatience*. We don't want fast because fast is actually better or cheaper. We want fast because someone convinced us that fast *feels more secure*. We have been told that fast feels *stronger*; feels *productive*. Fast makes the line go up and lines going up is a good thing.

But *fast* is affective and subjective more than it is objectively good. We have socially constructed why time matters and by extension we have socially constructed why faster things matter. And so the objective speed of something is actually secondary to our perception and understanding of speed. As anxiety-ridden animals, we have invented the want for things that *appear* fast, even if (by actual measurement), [things can be just the same speed or even slower](https://arxiv.org/abs/2507.09089).

We are taught not to like that our ideas and symbols are in-process, fragile, and flimsy... *and that we have to sit with that reality for a while before making something good and meaningful*. We want our ideas and symbols to appear as-congealed as possible as quickly as possible. Binary gender suffers from this problem! "Man" and "woman" are so strong and congealed and total and without nuance. *Yippee! We are safe from fluidity now, so long as we ascribe to a gender binary!*

And so large-language models give us *performative fidelity*; a sort of false, constructed faithfulness to ideas we haven't actually invested enough time into and haven't socialized. If anything, they construct loyalty to under-formed ideas more than they actually construct ideas, because constructing ideas is slow and messy!

Large-language models then simply become yet another social function of anti-fluidity, seeking to box up a thought as soon as we have it and transform that thought into a commodified, less-flexible unit, which we can claim is an "idea" that has been "prototyped" (without any symbol-making and socialization necessary!). This brain-fart-to-built-UI pipeline is so fast that it might actually begin to convince people that their lightly-sautéed neuron-events are actually really well-thought-out, mature concepts; *like slapping sheepskin on a lamb*.

"Prototyping is faster now" is yet another example of the make-you-feel-less-insecure style of marketing that every modern company dreams of taking advantage of. Marketing [sold us the need for deodorant by stoking human insecurity](https://www.smithsonianmag.com/history/how-advertisers-convinced-americans-they-smelled-bad-12552404/), and now it's working on the impatience and insecurities of software engineers, too.

<hr>
<br>

Note: Niklas Elmqvist's postdoc Gaby is actually running a survey right now on genAI use in visualiztion. Perhaps if you're reading this post, you can be convinced to [hop over and help them with their research by taking their survey](https://survey.au.dk/servlet/com.pls.morpheus.web.pages.CoreRespondentCollectLinkAnonymous)?