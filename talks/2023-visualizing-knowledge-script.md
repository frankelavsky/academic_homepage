# Practical lessons and resources from working in visualization and accessibility
### Frank Elavsky
Welcome, thanks so much for having me and thanks for the introduction.

I talk often about how we can make data visualizations more accessible for people with disabilities. But today, I will be taking a step back and giving a bit of a meta talk about myself and my journey doing this work.

---
# What is design?
As a designer, I would say that I believe I know less now about what design is and what it means to be a designer than I did 8 years ago.

In some ways, I recognize how much I really don't know now. There is so much left to learn.

And in a sense, I have more uncertainty now. And I mean that in the best way. 

---
## I am less *certain* than I was when I first started designing

And that isn't because I am less confident than I was in an emotional or psychological sense. I am much more confident. 

But I have learned and matured enough to know that 

---
# Design is an uncertain practice 

As a designer, I don't act out of knowledge. Design decisions exist somewhere between guesswork, existing knowledge, and pure dreams.

---
And really,
## All design involves a spectrum of *a priori* uncertainty and decision-making

I've been thinking a lot lately, what does it mean to design?

---

# What does it mean to be a *designer*?

Asking what design is is a harder question to start with than what does it mean to *be* a designer. From here, I can tell my story.

So, a while ago, I was a community organizer and a student of philosophy and theology. I know, probably the most annoying two things combined into one.

---
## Community organizing helped me see the power of social action
It helped remind me that

---
# Change is possible
We can hope and anticipate a better world and work to realize that hope.

And philosophy gave me a healthy sense of skepticism, while also helping me to recognize that

---
# There are many ways of knowing

But alas, philosophy and organizing didn't pay the bills. I'm disabled and need health insurance, so I left those behind for the tech industry.

Fast forward 6 years or so from my organizing days and now I am a computational support specialist at Northwestern University. I was research staff and helped folks all over the university visualize their research.

---

## 

## (a great technical achievement)

Back then, I believed that I knew what good design was.
And my projects were successful! Here in this project, I visualized over 1 million data points in SVG on the web. Technically speaking, I believed that was a good design. I was happy with it, so that must have meant that it was good, right? It was a great technical achievement and it was fun.

---

And researchers seemed to really value my work. Here is a screenshot of the 2017 nobel lecture on physics, that is Barry Barish, the recipient, using my visualization in his talk. As far as impact goes, I believed that was good design work too.

And not to knock on my past self too much. But back then, I was learning what I think a lot of designers learn at first: you learn how to validate what you're doing on your own terms and you learn what your immediate "customers" or "users" are interested in and find helpful or effective.

---
## And then I left and got a corporate job
At Visa

That was great work, but I was ready for something new.

Visa hired me to be part of a core group of staff level engineers and designers who would build a visualization charting library from scratch. This library was intended to support 2000+ developers and designers working on about 200 data products.

We wanted to build smart, declarative components that could scale quality design decisions, like accessibility to save others time and energy.

I now had to design and engineer a system that *other* people used to design. An interesting new step for me!

To build off of Moritz's talk, I went from spark work to ember work.

And back in 2018, a few other design systems had emerged for visualization, like IBM's. But our vision was the first to have robust accessibility built in from the start.

Accessibility was the majority of my intellectual work for 2.5 years.

---


Initially, colorblind safe palettes and alt text were all I thought our designers and developers needed. This was my background.

But Visa, a company that operates in virtually every country in the world, must comply with every country's accessibility laws.

The VGAR (visa global accessibility requirements) included 

---
## 126 accessibility criteria we had to pass

By contrast,

---
## WCAG (or the web content accessibility guidelines) have 78 criteria

And our first internal accessibility audit came in. We had significant work to do.

---

In the United States, 26% of people self-report living with a disability that affects their daily life. This is spread across a range of what are called "functional" categories of disability.

---

(Simplified image focusing only on visual disabilities)
I assumed that these were what we needed to focus on in our work, since we did data visualization.

---

But it turns out that every functional category of disability can encounter barriers when using interactive, dynamic data visualizations.

We were building pretty robust components that could be adjusted to fit the designs and functionality of pretty much anything you could imagine a standard chart being capable of.
And this was a big growing up moment for me, as a designer. I encountered my biases at a scale I never imagined before.

---
## My lack of knowledge had a tangible impact on who was included in visualization

---
## My biases created priorities, and those excluded some people

Now, let me talk about 

---
## Standards and guidelines
For a short minute. VGAR and WCAG gave me objectives.

And objectives can be good for design!

It's often hard to know where to start, where you're going, and to keep everything in mind while you're doing it.

I worked with the accessibility team closely to make sure our charting library was excellent, cutting edge even, in how we handled accessibility. I was pretty proud of it. We passed all 126 criteria! As far as comprehensive accessibility design goes, I believed I knew what was good design. It certainly checked all the boxes.

---

## 

## (Chartability's webpage)

In a separate talk, perhaps I'll tell a longer story about Chartability, a relatively big project of mine that has spanned the last few years.

This work at Visa on standards and guidelines are what inspired me to start making guidelines specific to visualization accessibility.

But back onto my journey at Visa: All seemed well with the accessibility situation

---
## Until we involved real users
I know this is not super deep or insightful to anyone who has ever shown something they've designed to another human who is supposed to use it, but after our research sessions I quickly learned that there was a lot of room for improvement.

We had expert users (data analysts, managers, and engineers) with disabilities help us better understand what worked and what didn't.

And I quickly realized a few things. First, that

---
## Standards and guidelines set the floor of an experience
But they don't ensure something is really good, or effective.

It should come as no surprise, but it turns out that people with disabilities are the ultimate source of certainty in accessibility.

---

This is an example of one of our design system components at Visa, a stacked bar chart using almost entirely default settings for color, spacing, typography, and accessibility.

In this particular example, I'm showing how we described a single bar inside of a stacked bar chart. This description is visually hidden but read by technology called a screen reader. Blind folks are the most common users of screen readers, but are not the only ones.

The text at the bottom shows the screen reader announcing Product Category: 2. Building: A. Count: 15. Stacked bar 2 of 3. This matches the visual tooltip on the chart.

And it turns out that blind folks who are expert analysts want information a lot faster than this. Native screen reader users often have their screen readers on very fast speed settings so that they can consume information as quickly as possible.

---
So this design worked much better for them. On the right, we've trimmed excess punctuation (which can often pause a screen reader) and made sure the most important information for understanding trends and comparisons came first in this string of text. When just trying to compare values, we dramatically sped up the time it would take them to make a comparison or dig for trends and patterns.

This example with text for screen reader users is just one tiny piece of design too, and it makes a huge difference.

Standards, the floor of experience, only get us so far. 

---
## Users teach us what a good experience is
Involving users with disabilities as early as possible, even as co-designers has been my practice lately.

After my time at Visa, I've since done quite a lot of consulting. And there is an emerging thing I've learned from people with different disabilities. And that is that

---
# Accessibility for some is a barrier to another

---

## 

## (chart textures can be a barrier for some!)

Just one example of this are chart textures. These patterns we put on charts, which we do because it is a standard requirement, might also become a barrier for folks with certain visual and cognitive disabilities. It adds complexity.

This happens a lot in design. In fact, data visualization itself is an attempt to make data more accessible for sighted individuals at the cost of losing textual richness that a screen reader user could access.

---
### A single, static design simply cannot *always* be accessible for *everyone*.

In disability spaces, "Accessibility for some that is a barrier to another" is called

---
# "Access friction"
Access friction is surprisingly under discussed in contemporary accessibility contexts (despite being common in spaces occupied by people with disabilities).

And why might that be the case?

---
## Access frictions challenge the notion of standardized access
People with disabilities talking about their real experiences should have precedence over everything else, right? Even standards?

Unfortunately, not in practice. Navigating access frictions will likely bring an entirely new generation of thought on accessibility in practice.

So at the beginning of this talk, I remarked that as a designer, I don't act out of knowledge

And I was being a bit tricky because in a way, I actually do. I've just always acted out of the knowledge I had at the time, even though now, afterwards, I can see that there was always far more that I didn't know than I thought I did.

I act out of knowledge but I act MORESO out of uncertainty and a *lack* of knowledge.

---
## I don't know what I don't know
But

--- 
## I'm pretty certain I don't know a lot of things

So first I believed I was certain because my designs worked for me.
Then, I was certain because others found them useful.
Then I was certain because I had really comprehensive guidelines.
And lastly, I was certain because what worked for a subset of a population should surely generalize if we have an adequate sample size.

But of course, 

---
# Access frictions bring us back to uncertainty

---
And so 

# Designing is a *way* of knowing

Now, I expect uncertainty.

And in fact, the most important part of design to me now is this anticipation that I experience. I am anticipating what happens *after* I design: I might find an opportunity to learn something new

So now, to me I've learned that 

---
# Design is an act of anticipation
And if I accept that and take a step back…

I see two kinds of design before me: designing that builds on my certainties, this is design that is slowly congealing into a model:

---

past experiences that become patterns can help us 

---


predict what to do in new contexts.

In this sense,

---

## Model-building is a *conservative* act.

I mean conservative here in the philosophical sense. It is an act of conservation.


The goal is to increase certainty and reduce risk: we use the past to try to predict the future.

But seeing patterns emerge and models form also shows another kind of design: 

---


the gaps. The empty space. The anti-models and the excluded things. The places we haven't been. The *uncharted* territory (pun intended of course). There is more uncharted than charted territory out there.

It occurred to me, if so much of what I do isn't actually truly certain.

Why not seek out those places we haven't been?

---
### Is the a better world always going to be built out of what we have already seen and done before?

Looking forward, two examples of uncharted territory for me are both related to access friction:

In my story, I am the designer. That is a common data point. If I was building a model, I'd predict that I'd continue to be the designer.

But what if in the future, I wasn't? What if we could design systems and experiences that give users the tools and resources to design for themselves?

What if we could explore a sort of

---
# "End-user design"?

I have a lot of uncertainty there, but I anticipate empowering users to enact change is part of a better world.

And the second idea I have for the future might be something that helps us realize end-user design, what I'm calling

---
# "Softer materials"

---

In contrast, concrete, and specifically concrete curbs, have been a tension point in disability advocacy, thought, and research for almost 60 years now. Concrete is physically hard. It is a tough material. We have to smash it and rebuild it when we want to cut curbs. Making a city accessible requires breaking the old to build the new.

But digital materials… those are much more fluid. I'd argue they are quite soft. Digital things are called *software* and not *hardware* for a reason.

---
## What if we brought the *soft* back into software?

What if our designs weren't static once they're done? What if others had the ability to change or morph the presentation, logic, or flow of our experiences?

Are there opportunities there?

I certainly anticipate that end-user design and softer materials will lose some advantages like convenience and speed compared to things made only by designers.

But what these new ideas offer is expressivity, control, and perhaps a way to mediate access frictions.

So to all of you, I want to encourage you to 

---
# Design with anticipation

Build a better world out of what you have seen before, use standards and research and experience. But also: look to those uncharted spaces and imagine what could be.

And of course, I hope that you all also try to make your visualizations more accessible too. Thank you.
