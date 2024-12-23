---
layout: post
title: "Strange avatars: Body-doubling with strangers"
slug: strange-avatars
tags:
- prototyping
- coursework
- user research
- avatars
- body-doubling
- strangers
description: I was assigned to build a little prototype and test it with users for a class. I chose to investigate what it might be like to facilitate a body-doubling productivity session between two strangers. But both of them looked like silly animals.
---
So this post is really a bit of a reflection on a recent assignment in Ken Holstein's *Prototyping Algorithmic Experiences* class. I was paired with a group of other students and we each set out to explore what it might be like to build a productivity tool that uses "[body-doubling](https://add.org/the-body-double/)" in some way. (We chose this direction as a group.)

Body-doubling is, in many ways, a concept and a practice that turns techno-individualism on its head. Rather than assuming the ideal outcome is that a person somehow has total self-sufficience when performing certain tasks, body-doubling reveals how powerful the social aspect of human behavior can be. For a great read on unpacking how *individualism* and *independence* can even be an ableist framing in technology research, check out [Cynthia Bennett's work on interdependence](https://dl.acm.org/doi/10.1145/3234695.3236348).

Body-doubling is a brain-hack that helps people be more productive and *in the zone* simply because they are working alongside another person. They don't really have to interact or hold each other accountable at all. There is just a shared understanding that the time they have together is for getting stuff done. Communities who are ADHD, autistic, neurodiverse, and/or have [executive dysfunction](https://add.org/executive-function-disorder/) have really spearheaded this practice, especially in recent years. It's wonderful.

But of course, body doubling is something generally done in person with someone else and typically you know them. But are there ways we could imagine some kind of body-doubling on-demand? Like you just need to set aside some time to get work done and don't really want to go through the trouble of planning and coordinating with a friend? (Keep in mind, *executive dysfunction* is something that folks who love body-doubling struggle with!)

## Challenges and Goals
So I wondered: what if your body double was a stranger? And what if there was some kind of match-making magic that just paired you with another person? (As a note, someone else on my team was exploring what that *magic* might look like as their contribution to our parallel prototyping.)

I believe this might help with fast match-making, taking away much of the executive difficulties of coordinating a session. In addition, this could also help facilitate on-demand productivity, which might actually benefit and compliment some [ADHD productivity habits](https://www.reddit.com/r/ADHD/comments/mtlmp5/are_spontaneous_bursts_of_productivity_common/).

In particular, the fact that some ADHD folks are highly productive in short, unpredictable bursts is not something I wanted to frame as a negative trait or design against. Most self-help and pseudo-science literature on productivity talks about regularity and self-sufficient, consistent, commitment as cornerstone behaviors of productive people. Instead of following this assumption, I wanted to imagine how to empower the existing productivity behavior of ADHD folks through on-demand body-doubling. Essentially I'm asking, "can we *enhance* existing ADHDer's spontaneous hyper-productivity behavior?"

HCI research especially has a habit of imagining and designing technology according to normative standards that try to enforce "ideal" human behavior and outcomes (such as holding people with disabilities to conform to neurotypical, medically non-disabled, and/or capitalistic behavior, further reading: [1](https://dl.acm.org/doi/abs/10.1145/3544548.3581480), [2](https://dl.acm.org/doi/abs/10.1145/3544548.3581556), [3](https://dl.acm.org/doi/10.1145/3432245)). This approach to and motivation for technology and innovation is often an ableist, medicalizing framing, despite its wide popularity. I wanted to avoid assuming someone else's existing behavior is bad and rather just investigate how to enhance body-doubling.

So! If you were paired with someone who was a stranger, there are some potential issues we need to consider. First, is that you might not feel safe or could be uncomfortable having to introduce yourself or interact according to social expectations of some kind. What if the other person is racist or sexist? What if you don't feel fully able to be yourself and instead want to [mask](https://add.org/adhd-masking/) in the other person's presence? And of course, I reckon that we might run into what I'm dubbing "the Omegle problem" (obscenity, nudity, offensive behavior, etc).

So I wondered: what if we weren't really ourselves in these spaces? And what if what we could do when we interact with others was limited to a set of certain actions or behaviors?

First, I took inspiration from [VTubers](https://en.wikipedia.org/wiki/VTuber) or "virtual youtubers." These are avatars (typically custom 2D or 3D character models), rigged with facial-recognition capabilities. VTubers will typically stream or create online video content appearing as this character. And due to their popularity, some companies even feature Vtuber characters as official spokespeople or mascots.

My assumption is that if everyone looks different than their normal selves, they might feel less obligated to act according to particular social conventions, may feel safer being themselves, and have less opportunities to be prejudiced towards their partner. I reckon this will have a positive impact on their experience and productivity (that's my conjecture, at least).

<figure>
    <img src="https://www.frank.computer/images/gawr_gura.png" alt="An anime character who is wearing a shark hoodie. Behind them is a screen that says All about bloop (with bloop written in scratchy hand-writing). Just the facts! Name: Gawr Gura. Birthday: Jun 20. Age 9927. Height: 141cm. My favorites! Color: Blue. Food: Salman. Likes: Food. PWWIE. Dislikes: Hot sand. Biggest fear: Loud Stomak."/>
    <figcaption><a src="https://www.youtube.com/channel/UCoSrY_IQQVpmIRZ9Xf-y93g">Gawr Gura</a>, considered one of the most popular, family-friendly Vtubers on YouTube. Screenshot taken from her debut video stream.</figcaption>
</figure>

And to help keep activity regulated and safe, I drew inspiration from online multiplayer video games and the concepts of avatars with emotes: in games, such as World of Warcraft, Fortnite, or the indie game Lethal Company, players look like in-game characters but have a limited set of actions that they are capable of making.

<figure>
    <img src="https://www.frank.computer/images/lethal_dance.png" alt="Two players in Lethal Company, dancing. They are wearing their company-issued hazmat suits. Their dancing looks awkward and dorky, which is likely an intentional design choice by the game developers."/>
    <figcaption>Players using the "Dance" emote in <a src="https://en.wikipedia.org/wiki/Lethal_Company">Lethal Company</a>, an indie game about salvaging in horrific conditions for an even-more-horrific space-capitalist mega-corp.</figcaption>
</figure>

So my idea: What if we used the facial recognition features of Vtubers to help make avatars feel alive to maintain a sense of presence with another person, but limited what other actions the avatar was capable of, in order to help participants stay focused and productive?

## Strategy

**The pitch**: We pair strangers who body-double to get tasks done, but they each appear as animal-themed vtuber avatars. Their avatars cannot speak but track their facial movements, head direction, and expressions. There are chat capabilities and the option to send emoji (of a limited set) to the other participant.

Participants have to type out a sentence to the other at the start of the session that explains what they hope to accomplish in 10 minutes, and then can focus on their task.

After the 10 minute session, I send participants an email with follow-up questions.

My goals for this prototype are really to get a sense of the "experience extrema" (the best and worst ends of my hypotheses):
Investigating my most negative assumptions:
Are avatars distracting? Disruptive? Is it still off-putting or nerve-wracking to body-double with a stranger? Do people feel unsafe? Is the regulation of interactivity stodgy, robotic, or impersonal feeling?

And my most positive assumptions:
Are avatars fun? Do people feel safe? Are the participants able to get their work done? Do they enjoy the experience? Can avatars help disarm or dissolve potenially distracting differences between people, such as language, culture, or otherwise?

Luckily, Zoom actually has a feature for desktop users where you can enable pretty good avatars, which will allow us to test our vtube-atar prototype as a realtively high-fidelity, working prototype. We won't have close control over the environmental factors, but it lets us really explore the avatar portion with working facial recognition and relatively cute choices of animals.

I had volunteers (both from class and also my personal social network) sign up, and I paired them with strangers (folks they didn't know).

<figure>
    <img src="https://www.frank.computer/images/vtubatars.png" alt="A polar bear and a rabbit participant in a call together. In chat, laezel the bunny hehe wrote: i need to write an email to my mom about how to buy a new phone. anon wrote: I want to turn 10 recent emails in my inbox into 0 emails (by responding to them). laezel the bunny hehe responded: we emailin O.O. and anon wrote back: Aw yeah."/>
    <figcaption>Two participants, starting their session together.</figcaption>
</figure>

## Findings
Overall? The prototype was a success. Folks had fun and were able to complete their tasks as well. Response to the avatars helped provide some supporting evidence for some of our positive extrema hypotheses.

Of course, since this was for a class project and the prototype sessions were relatively long (about 20 - 30 minutes from start to finish, including setup, working, and follow-up), I only had 4 total participants. Interestingly, without prompting or asking, 3 of the 4 participants self-identified as neurodivergent in some way when we mentioned this was a body-doubling prototype experience. I didn't ask the 4th whether they were or not, but it is good to know I managed to select participants whose feedback would be valuable for this kind of activity.

I'd love to further this prototype and study, especially to explore more deeply potentially negative downsides (a sort of experiential risk assessment, if you would).

Some of the questions and responses from participants (all anonymized here, I just selected some of my favorite responses):
### Did using an avatar make you feel more or less comfortable when co-working with a stranger?
- "Way more comfortable! Based on my past experiences with body doubling: I expect that I would have been more self-conscious otherwise, and would have felt more responsible for managing a social interaction."

### What are your thoughts about lack of talking? Did that help you focus? Did it feel impersonal?
- "I understand why there is a lack of talking, and I think it was helpful for focusing. It would be hard for me personally to not be distracted if there was "mysterious" background noise or voices."
- "Controlling environmental noise is important for me when I study and work. I also think a lot of my focus would go toward making sure I don't disrupt another person. However, it would feel impersonal if the person I was with didn't engage at all through chat. Seeing the avatar move also helped it feel more like a real person was there vs just some robot."
- "I'm glad that we were asked not to talk. I think it was important for me not to attend too much to the particulars of the stranger (not hearing their voice helped with this), and also not to have to dedicate too much of my brain to thinking about how I look or sound. I think it helped me focus. I base this on my past experiences with body doubling, where it always takes me a while to "recover" and re-focus when another person makes eye contact and talks to me. In this experience, by contrast, there was none of that. But I still got the benefits of body-doubling!"

### How did you feel about the emotes? And text communication? Did you feel motivated to chat or type to the other person? Was it distracting?
- "I enjoyed the text communication and emotes because it makes the experience less isolated while not being entirely consuming. I am also used to this type of communication format within a community space. It was nice to see a chat response pop-up every now and then when I would look up from my work - like a little treat."

### Were the avatars fun or funny? Enjoyable? Interesting?
- "The avatars were fun! I thought being in "cute avatar mode" made my task feel more enjoyable. I kept thinking: "Look at that cute lil' animal co-working with that other cute lil' animal. Oh wait, that's me!" I'd much prefer answering a bunch of emails as a cute animal avatar living in a void, versus as myself."
- "The avatars were really fun, funny, and cute. I enjoyed watching my own avatar as well as my partners to see what they were doing."
- "The cow avatar is mvp."

### Did you feel distracted or like the mood wasn’t serious enough for working on your task?
- "I wasn't distracted - it was very easy to focus. I actually usually seek out a whimsical, fun mood when completing work tasks. So this was perfect."
- "Initially, it can feel not too serious when you first experience an avatar and how it tracks your facial expressions, head position, etc."
- "I definitely wanted to play around a bit at first. Once that novelty wears off a little, it's not distracting, but more feels comfortable."

### How would you feel about sharing your own screen? Do you feel that would be important or necessary for the exercise? What concerns would you have about sharing?
- "I would not feel comfortable sharing my screen with a stranger."
- "Probably wouldn't want to do that, I'd have to worry about a lot if I did that."

### Did you feel it was necessary or helpful to type out what task you were trying to do before you started? What advantages or disadvantages do you feel come with disclosing this?
- "Typing out my task was helpful because it gave me a focus and purpose. It's also fun getting feedback from the person I was chatting with."
- "I see it as an advantage in that it's a helpful reminder for myself to be accountable. I also don't see it as a disadvantage because I get to choose what and how much I share about the work I'm doing. If I was intentionally procrastinating or trying to avoid doing my work, then sharing my task could feel bad."
- "Yes! I always find this helpful in co-working sessions because it helps me reflect upon what I most want to accomplish during the session. I then feel somewhat accountable for completing that task (or tasks). I feel that I can always choose to disclose as much or as little information as I want about task(s). So I don't see any disadvantages, personally."

### Additional remarks (unprompted)
- "Oh as some feedback, I really wish I could have customized my avatar more! It was really cute but wasn't totally me. I'd love to have a big bow or some makeup or maybe different clothes."

### Other findings and thoughts
Well, controlling the environment with zoom had a few unexpected accidents. Namely, a participant accidentally turned on their mic at one point and a participant in each session still had their profile picture shown (which meant they weren't totally anonymous).

<figure>
    <img src="https://www.frank.computer/images/moovatar.png" alt="A racoon and a cow participant in a call together."/>
    <figcaption>The cow's highlight ring is showing, meaning their microphone was broadcasting. Profile pictures in chat have been scrubbed from this image, but in the original one person had a selfie of themselves shown next to each message they typed into chat (zoom's default behavior).</figcaption>
</figure>

Of course, this was a prototype but in the future it would be great to use a higher-fidelity prototype that doesn't rely on zoom, one where we can control the environment more carefully and also automatically anonymize our participants. Set-up was significant work for one participant in particular who actually had to update their zoom client (which they hadn't done in a while), taking nearly 15 minutes total just to get started.

Also, we love the idea of exploring personalization more with the avatars as well as intentionally pairing participants who don't speak the same language, to see if translation-bots or assistants can help bridge gaps in a natural way that doesn't feel distracting. I think that having avatars capable of waving, dancing, cheering, or performing some other simple actions with their hands or arms also might be worth exploring further as well. Oh, and profile pictures should reflect the person's current avatar too.

## Meta-reflections
Of course, because this is me and I'm gonna do my thing, I've been stewing a bit on our exercise (which is to explore productivity + technology + algorithmic experiences). Here's where I do some navel-gazing, after watching other groups present their work.

I think it is really interesting that in this productivity exercise, many of the other students in our class carry some assumptions about what productivity is or how to frame their problem or solution spaces. For example:
- There are normative "good" things that people should conform to (such as concepts like "self-motivation")
- Continuing that, individualistic productivity is an ideal outcome (people should be productive all on their own)
- The idea that "intrinsic" motivation is even real (cognitive science would argue that most all cognitive activity is a result of external stimulus in some way or another, whether based on present, past, or future stimulus or imagined stimulus)
- A lack of productivity is *bad* (perhaps the exercise itself motivates this) and should be "solved"
- "Habits" are intrinsically related to productivity (what even IS a habit?)
- The experiential neutrality of tech intervention (IE, that a pop-up or reminder isn't good or bad, painful or wonderful, it's just neutral)
- Why some people experience a lack of productivity (behaviorally), for example having low-dopamine production or response (like ADHD), intersections with poverty or abuse or other socio-economic factors, negative associations with failure/inability or starting/finishing something, perfectionism/OCD, lack of social support, chronic illness, lack of interest/stimulation, or depression.
- Historically, what factors have contributed the most to productivity (war, colonialism, Protestant guilt aka the "Protestant work ethic," funding, egalitarian revolution, managerial capitalism, etc).
- Socially/personally, what conditions are when people are/have been most "productive" (caring for a newborn, when playing a video game, when working a job, when you have an administrative assistant, etc)

Having assumptions isn't necessarily bad, per se. We all have them, of course. But I think that good prototyping comes about when we are willing to question our assumptions. Really novel, spicy and provocative ideas emerge when we are willing to interrogate our most formative assumptions about our own values, understanding, and intentions. I'm wondering if there could be some kind of way to teach students (or have them learn by example) what questioning your own assumptions can look like, without falling into some Philosophy 101 course. Or perhaps, as things tend to be with me, all roads lead back to philosophy eventually.