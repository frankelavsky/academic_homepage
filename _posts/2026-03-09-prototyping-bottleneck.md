---
layout: post
title: "On LLMs: Was prototyping really a bottleneck?"
slug: prototyping-bottleneck
tags:
- prototyping
- design
- software
- llms
- large-language models
- ai
- agentic models
description: "I keep hearing folks claim that the fact we can 'prototype' so quickly now is a good thing. But what if the slow parts about prototyping were actually good?"
---

(This post is a part of my new mantra moving to Cal Poly SLO: "move SLO and repair things," which is in direction tension with the mantra from the tech industry "move fast and break things" as well as a play on the abbreviation of San Luis Obispo, where I will soon work. I want to cultivate a research culture and lifestyle focused on maintenance, careful deliberation, and *care*, as defined in the feminist sense of the word.)

Ever since ChatGPT, folks have frequently remarked something along the lines of, "LLMs are so fast, now we can easily scaffold prototypes! Finally, the bottleneck is gone!" *Bottleneck?* Was the problem with prototyping the fact it took too long? Some nerd (Microsoft guy maybe?) said the even-more-ridiculous "finally the bottleneck from typing is gone" as if the speed of typing is what was holding back new ideas and features and improvement and so on.

<blockquote class="warning">
    <p>⚠ <b>Warning</b>:</p>
    <p>This blog post is a response to a post on LinkedIn. The original may someday be lost in time! For now, the <a href="https://www.linkedin.com/posts/ebertini_i-am-convinced-we-are-in-a-new-era-for-visual-share-7436798122770653184-CZpP?utm_source=share&utm_medium=member_desktop&rcm=ACoAADDAwBkBOdoW11I9B5DHy57VfR5jIs33Kq0">post is here, by Enrico Bertini</a>.</p>
</blockquote>

Enrico writes,

> "I am convinced we are in a new era for Visual Analytics (VA) (i.e., visual interactive data interfaces), but I am not sure we have yet realized it.
> In VA, building and refining a prototype has always been a costly bottleneck. This is no longer true. A single skilled person can build a working prototype in a matter of hours. They can also thrash it and rebuild it within hours. Heck! They can even build three alternatives and show all of them in maybe 1-2 days. This is no small change. It's massive.
> How do we deal with that?
> All of a sudden, an idea in my head can be transformed into a tangible prototype very quickly. This has enormous implications for applied research. If I work with a partner in a specific domain, I can quickly show something rather than talk. If I am good enough, I can even build something they can use pretty quickly.""

My response:

In some contexts, prototyping is probably a "bottleneck" but prototyping is also central to generating an understanding of the thing you're making, questioning your assumptions, and trying to communicate the rawest components of your ideas.

In terms of idea+prototype "fidelity" (understood as "faithfulness") I reckon we need to now consider: whose ideas is this prototype faithful to? Is this prototype faithful to the original human creator, or are there embedded biases in this prototype's function and construction because it was made using agentic tools/modern models? An "unfaithful" prototype (what we call "low fidelity") now has a new meaning, because we can more easily create prototypes that appear to be high fidelity, but may not actually be faithful to the intricacies of any particular idea at all.

This line, in particular, I think *does* have enormous implications for applied research, but I wouldn't necessarily assume that the implications are all good.

> All of a sudden, an idea in my head can be transformed into a tangible prototype very quickly. This has enormous implications for applied research.

I agree that a shift is taking place. But I don't think we should just move forward as if the act of slowly prototyping itself was a problem to solve. I would argue that the act of prototyping (*especially* when done slowly) is still valuable as a necessary step we take as creators, attempting to make something new. (As a note, I get disappointed with the view that a "prototype" is the same as "a first attempt to create something" and not "an artifact I use to reflexively to discover+congeal my own ideas and communicate with.")

I've written about prototypes before, and what I think much of our literature misses on the subject: that prototypes are actually a tool for *communicating*. ([This blog post of mine on prototyping](https://www.frank.computer/blog/2024/01/what-is-a-prototype.html) was my most-visited post, before [my post on AI + Tools](https://www.frank.computer/blog/2025/05/just-a-tool.html) came out. Funnily enough, *this* post I'm writing right now seems to be marrying the two.)

The fact that we can build functional symbols communicating *faster* isn't necessarily good, if we don't have a firm grasp of the idea itself in our head in the first place. One of the best parts about prototyping, to me, are the slowest parts: you draw something out with a pencil and paper, you cut out pieces of cardboard, you use some lego bricks to scaffold something, you get up to a whiteboard with a few other people and start squaking your pens across the blank canvas together... *and you talk about that stuff with each other.*

"Prototyping" is *not* a linear pipeline that goes from an idea in your head into a material artifact that represents that idea.

**Prototyping is a method of symbol-making. And we use those symbols to communicate ideas.**

And this is why I am actually worried about prototyping that moves *too* fast. And in fact fast-prototyping-as-a-problem isn't new! Researchers who studied "fidelity" in prototyping have long discussed how moving too quickly to higher fidelity prototyping can bias your future ideas, bias your outcomes, and ultimately produce *more* costs, not less, down the road (see this [seminal summary of the great older battles on fidelity by Rudd, Stern, and Isensee](https://dl.acm.org/doi/pdf/10.1145/223500.223514)).

So back to Enrico's argument here... I'm not sold that faster = better and *certainly* not sold that faster = better = cheaper (specifically responding to the sentiment in his post that it has "always been a costly bottleneck"). I think that existing literature would argue quite the opposite. Faster = 1) more assumptions are missed in the core ideas, 2) ideas that appear already-refined become immune to questioning, and 3) faster, more-refined prototypes are ultimately less social.

*Yes!* You heard me: Faster prototypes mean *anti-social* prototypes. This final point (which I am making, not necessarily something I've read in the literature on this) is actually the most important one to make (which I've already brought up earlier): but that **prototypes are about symbol-making for the purpose of communicating**. If you were the only person left alive on this earth, but you still learned how to speak, you would likely not lose your internal dialogue. You would still speak, even to yourself, to think through things. And prototyping, as an act and process (not a destination), is about that symbol-making. You're working through whatever idea needs forming and needs new symbols for expressing. Prototypes are a form of self-socializing ideation. And their inherently symbol-rich, generative nature makes them idea for socializing with others.

But inviting someone to write a language with you is different than asking someone to critique a sentence you wrote. Prototyping that is low fidelity (and slower) is the first kind. Higher fidelity (with LLM assistance or otherwise) invites the second. We *want* socialization on the core symbols and ideas we choose to construct! And that might always have a *human* bottleneck built into it (for as long as we humans are in charge of prototyping, that is).

But just to drive this home: ***socializing your idea* is the real value of a prototype**. Socializing a raw idea is a fundamental epistemic activity that we do. And I honestly wouldn't like ideation, as a human act, if I only ever did it alone or with a machine that simply confirms my biases and listens to my instructions. Refining, discussing, sharing, mixing, appropriating, and fusing ideas are actions that really only come into the picture once we have a prototype in between a few people who are trying to figure something out together.

But *why* is socializing so important? Because our intelligence is *positional* and *situated*. We have "horizons" of knowledge, and limits, as singular beings. We are not objective. Yet through social inclusion in the act of making and forming ideas, we broaden the angles and horizons of our social constructs. And for this reason, prototypes that are socialized are simply better, more meaningful creations. I'd even argue that a prototype that isn't socialized isn't a prototype at all, it is just an early attempt at making something: the focus is on the *object* being made, not the idea it represents. And it's that human socialization and collective meaning-making that turn an artifact-in-process into a prototype that is refining something outside of itself: an *idea-in-process*.

In "[what do prototypes prototype?](https://hci.stanford.edu/courses/cs247/2012/readings/WhatDoPrototypesPrototype.pdf)", Houde and Hill argue that the separation of artifact and idea is key to understanding the value of prototyping: the prototype isn't the idea itself, it is just a symbol of the idea (hence, why I write about why fidelity = faithfulness and not something like "quality").

I worry about prototypes that are *too* refined *too* soon. Will they alienate our ideas, because our ideas are less inviting for critique/reshaping at fundamental levels? (Isn't it ironic, that using a *language model* possibly holds us back from building a truly social new set of symbols for communicating an emerging, shared space of thinking?)

Anyway, this blog post is a largely-unstructured brain-dump in response to a linkedin post. Thanks to Enrico for posting it! It certainly got my juices flowing.

And it *does* seem ironic to me to socialize the idea that prototyping=faster=cheaper=good (that all of these things are true and related). That seems like an idea that has been developed *too far*... it has too much fidelity, not enough prototyping. Perhaps I would recommend going back to the drawing board and re-assessing this?