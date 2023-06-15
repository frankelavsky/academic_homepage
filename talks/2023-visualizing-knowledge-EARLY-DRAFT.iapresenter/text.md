# Practical lessons and resources from working in visualization and accessibility
### Frank Elavsky
Welcome, thanks so much for having me and thanks for the introduction.

I have hopefully seduced many of you with a purely utilitarian sounding title for this talk, which I hope not to disappoint. I'll bring you along a journey and share some practical lessons and resources from my work in visualization and accessibility. But also, within this is a thread of something somewhat philosophical I've wanted to share for quite some time.
---
# What is art?
This might seem like a strange question to ask at the start of a talk on visualization and accessibility. But bear with me. This question is related to the much more relevant question "What is design?" That I hope we can stew on in my presentation.

So, what is art? I recently re-read an introduction to the Left Hand of Darkness by Ursula Le Guin and in it she remarks, "a novelist's business is lying. I talk about the gods; I am an atheist. But I am an artist too, and therefore a liar. Distrust everything I say. I am telling the truth." I love this so much.

In a very provocative way, she isn't just saying what art is, but describing the power of a metaphor. She is describing her own work and what she has made it. There are many artists and novelists who don't write the way she does, but she speaks about her own ideals and her own craft.

She isn't just saying what art is for everyone, but what it means for her, and in a way, what she wants it to *become*.

So for that, I ask
---
# What is design?

# 

Or more specifically,

---
# 

# What do I want design to *become*?
What does design mean, *for me*? I am just going to open with these questions and I hope that you all chew on them while I wander through a telling of my journey these past few years. I'll come back to this at the end.
---
## I got a corporate job at Visa
And my entire career shifted. I went from caring about accessibility to doing it almost full time.

Visa is a global company that operates in virtually every country. And because they work closely with banks and governments, accessibility is a requirement for every product. But they don't just comply with a single country's laws, so their internal design team came up with VGAR, which is a set of 126 accessibility requirements. By contrast, WCAG (or the web content accessibility guidelines), which is generally considered to be the largest and most used set of accessibility guidelines, only has 78 criteria in their 2.1 version.
---
## I was brought on to help build a charting library
And this library had to comply with all these criteria.

We had a rough first review in early 2019 and I shifted to almost exclusively devoting my intellectual energy for accessibility.
---
## We had a lot of "ability assumptions"
It is incredibly common for folks who are aware of what accessibility is in visualization to, at a bare minimum, think about color and color vision deficiency.

My accessibility journey as a visualization engineer and designer was primarily focused on visual disabilities up until this point.
---
## Keyboard access and contrast
(Examples)
In academic terms, the assumptions designers have that shape their decisions can be called "ability assumptions." When starting out, designers often assume that others are like themselves. And of course, maturity as a designer is recognizing other people exist in the world who aren't like us.
---
## But these assumptions create *bias*
And bias in design is a set of assumptions that have priority, power, and agency, often to the detriment of real people who are forgotten or excluded.
---
## So I had to grow up as a designer.
---
# 
It turns out that data visualization as a practice can produce barriers for virtually anyone with any disability.
---
# Chartability tried to meet this need
Because of this, I started consulting in my spare time. I realized that comprehensive consideration for accessibility in visualization was long overdue. And our field as a whole needed to do something about this. So with the help of many friends and colleagues with disabilities and without, I came up with Chartability.

This project, which most folks who are familiar with me know about, is a set of accessibility guidelines that are specific to visualization.

I actually still work on this project too.
---
## Meanwhile...
Back at Visa, something really obvious and important happened that I want to briefly touch on:
---
## We involved users with disabilities
And hoo boy, did we learn some things really quickly.

Now, there is a really important phrase in disability organizing that comes from advocates pushing for the Americans with Disabilities act. And that is,
---
# "Nothing about us, without us!"
This statement means that decision-making, and really, ultimately, what makes something accessible, comes down to whether or not people who are disabled are involved.
---
## And our accessibility experiences could be improved
Unlike our ability assumptions producing biases that made us completely disregard something like keyboard accessibility, instead we had a set of assumptions about what a good experience actually was.
---
## Text
Text rules all. And to a screen reader user, text is the primary way to consume almost all information.

We had a particular way we ordered and arranged the alt text for elements inside of a chart. And it turns out that expert analysts and users wanted to be able to get insights as quickly as possible.

---
## Removing, improving
What that mean was really removing excess punctuation that largely only serves visual conventions, and also making sure the most relevant information is as early as possible in a given string of text.

So, my biggest lesson in this was simply that
---
## Standards and guidelines can give us objectives...
Which is good!
---
## ...but they don't help us understand what is *effective*
This was a significant shift in my thinking.

Standards are good! But they are the floor of experience. We need to strive for excellence. And we get there by doing accessibility work...
---
## *with*, not just *for*
*with* people with disabilities, not just *for*

---
# 

So one day in 2020...
---
## My phone broke
*This* phone! I got a security update and the contrast stopped adjusting automatically because of a hardware failure. I had paid for my phone in full up front and stubbornly refused to buy a new one.

But losing automatic contrast adjustment is serious.

The contrast on your phone is a setting that adjusts how bright the screen is. Using sensors on the front up here, my phone screen should brighten when it is bright out and darken when it is dark.

Seriously, I took for granted how hard a phone is to use without this feature automatically doing its job.

And a few months after this happened to me, and I was beginning to accept that I would be squinting at my screen to find the contrast bar to brighten it at least once a day, I saw...
---
## 
this graphic shared by someone else on social media. I'll break it down, but first a little background:

Inclusive design has a saying "design for one, extend to all."
---
## This comes from curb cuts
And something called the "curb cut effect," which is a phenomenon that researchers have been talking about for decades.

The phenomenon is this: cutting curbs, which was first done for folks who use wheelchairs, actually has broad social impacts that are good for almost everyone else. Cutting curbs makes streets safer for everyone, from people carrying groceries, walking kids, to the elderly.
---
## 
So let's go back to that image and zoom in. What the Inclusive Design 101 folks at Microsoft are showing here is that there is a temporal and situational aspect to disability. Someone might be permanently missing or unable to use a limb. But someone might just temporarily lose motor function, like they broke their arm and have to wear a cast for 4 months. And someone might be situationally impaired, like working on the computer with one arm while holding your newborn in the other.

When you design with and for a person who has a permanent disability, you learn things about their needs, behaviors and strategies that can help make your accessibility excellent. And the peripheral effect is that these things you've designed can help others who might just be experiencing temporal or situational impairments.

This opened my eyes to two new ways of thinking about accessibility and design.
---
First, that
## Disability is *produced* in the spaces between bodies and our world
And that
---
## Selfish accessibility is valid

So first,
---
## Disability is *produced* in the spaces between bodies and our world
My phone, this little piece of technology, can produce a barrier for my use if the sun is too bright and this technology doesn't adapt.

The sun, my phone, and my eyes all have a relationship here.

And going back to my first story about community organizing, I want to tie in the social model of disability with this realization:
---
## I can't change someone else's body to fit my expectations of what a normative "user" is.
And I shouldn't! That is what disability studies calls "medicalizing" people's bodies and it is generally not good.
---
## But I *can* work to remove barriers.

When I was an organizer, the real problems (big P problems in the world) were often things we could *never* change. The crushing realities of capitalism: the laws that enabled the slumlord to take ownership of 4 city blocks, the failed policy and investment in publicly-owned utilities, and a mayor who only cared about the success of their own career.

What we focused on were things that we had the power to win. This goes back to the social model of disability:
Social action can bring a city to cut curbs, rather than expect every wheelchair user to remain on one city block their whole life.
---
## We can't put the burden on our users
*We* build data visualizations. We are like the city architects and designers and engineers. We should be the ones to cut our own curbs, the curbs we create. Our environments are things that we can and should do something about.
---
## 
It might seem obvious, but this little graphic turned on some lights in my head that connected my past to my present: the responsibility falls to us, the makers, to remove barriers and avoid making them in the first place.

And the second thing I mentioned was
---
## Selfish accessibility
Adrian Roselli coined this term. Adrian explicitly argues that it is good to motivate your accessibility work on the grounds that you are helping your present or future self.

Folks often remark that they care about accessibility because they have someone close to them who is disabled. And that's a wonderful reason to recognize that this work is important.

But also: doing it for yourself is a good reason too.

In the same way that commenting your own code is good for yourself in 6 months as much as it is for someone new to your codebase,
---
## disability comes for us all in some way
Eventually.

We might not end up holding a newborn while working or break an arm in our lifetime, but most of us will probably life to an old age. And age is the ultimate equalizer. Accessibility will matter to you someday just like it matters to one and a half billion people today.
--- 
## Now what?
These are all lessons that to me, have become foundational for my thinking.
---
## Ability assumptions create bias
---
## Guidelines give us objectives
---
## Accessibility work *with* not just *for* helps us understand what is good
---
## Barriers can be produced in the world *we* build
---
But
## We have the power to remove the barriers we build
---
## So: what do I want design to *become*?
Well, I've been stewing on something called "access friction" a lot lately.
---
## Access friction is when accessibility for one is a barrier for another
---
# 
This made me realize that there is an epistemology problem in design writ large.
We can't know what is a good design just based on our own use
We can't know what is a good design just based on standards and guidelines
We can't know what is a good design just based on what one user or group of users find effective
---
# Design is filled with uncertainty
But that uncertainty is also a place for growth, a place for opportunity, a place for anticipation.

But what design itself means can also change.

So,
---
## What do I want design to *become*?
Right now, we mostly make things for others.
---
But
## What if the future involves *end-user design*?
What if out of the space of negotiating access friction are opportunities to imagine how to empower users to easily and effectively change the systems we build to suit their needs?

If a single design can't help everyone, what if people had what they needed to help themselves?
---
And
## What if the future involves *softer materials*?
I think this might go hand in hand with the previous idea.

Concrete curbs are physically hard. They are solid. They are heavy and dense. Some things we design, like laws and physical spaces, are very difficult to change.

But the digital materials we already have are much softer. So why don't we explore how to use these softer materials?

If a static design can't help everyone, then what if we don't use static materials?
---
## Will either of these ideas come alive?
I don't know. But I am anticipating that *something better* is coming. And I want to be part of it.
---
So to me,
## Design is an act of *anticipation*
We *embrace* uncertainty. We *anticipate* change. And yet we still choose to do something.

And I hope that all of you can be inspired to really see that accessibility work *is* design. I hope that you all embrace the uncertainty in our work and design as if you *anticipate* a better world.
---
