---
layout: post
title: "Minimalism and the absurdity of the data-to-ink-ratio"
slug: data-to-ink
tags:
- tufte
- data
- visualization
- minimalism
- data-to-ink ratio
description: "How much minimalism is too much minimalism? I explore this question and propose the most minimalist, highest scoring data-to-ink ratio on a visualization ever made as a thought piece. Why? Well novices learning to make data visualizations are often taught to avoid 'chart junk' and strive towards visual minimalism. But they aren't told when to stop."
---

Edward Tufte's books, "[Visual Display of Quantitative Information](https://lmscontent.embanet.com/USC/CMGT587/Tufte%20Ch2%20and%205.pdf)," "[Envisioning Information](https://journals.lww.com/optvissci/citation/1991/04000/ENVISIONING_INFORMATION.13.aspx)," "[Visual Explanations](https://www.ntf.uni-lj.si/igt/wp-content/uploads/sites/8/2015/09/Oblikovanje001-1.pdf)," and "[Beautiful Evidence](https://pages.mtu.edu/~hcking/Tufte_hKing.pdf)" combined have [29,010 citations](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C39&q=edward+tufte&btnG=) as of April 22nd, 2025 on Google Scholar. To say that Tufte has been influential in the field of data visualization would be an understatement. Few others have contributed as much impact as Tufte to the spread of ideas related to my field of work.

Tufte has 2 specific ideas, both fixated on the design philosophy of minimalism, that I'd like to discuss in this piece: "chart junk" and his "data-to-ink ratio." "Chart junk" is a label given to visual decorations that are considered superfluous, meaningless, and even harmful to the central function of visualizing data. And the "data-to-ink ratio" is a rough heuristic for maximizing the information that a graphic can portray in as little "ink" (visual marks of any kind) as possible.

Both of these ideas have been hotly contested in the visualization research literature. How do we really know whether visual decorations are harmful? First, how do we even consider something is "chart junk" and then second, how do we observe what effects chart junk actually has? And with the data-to-ink ratio, how do we objectively measure what data is, and then how do we accurately measure the ink used to communicate that data?

Exploring these questions has been about as effective as bringing a squirt gun to fight the ocean. Empirical research (unlike Tufte's opinion-based approach) has comparatively nearly 1/20th the collective citations as Tufte's thoughts. Even if researchers are right in questioning easy, un-nuanced design notions like "chart junk" or the "data-to-ink ratio," we are virtually powerless to stop the force of Tufte's immense existing impact on how people think about visualization.

## If you can't fight the death grip of minimalism on modern thought... can we embrace it to the extreme?
So perhaps we cannot "win" in the marketplace of ideas against someone like Tufte. Easy-to-recall rules that make young professionals feel like they have powerful expertise over a complex domain like visual design are hard to conquer. Essentially, asking for measured, mature designerly consideration is simply not as popular (and perhaps never will be) as giving someone fast, naive design heuristics.

So what if we just take Tufte's idea as pure law? What if we made a visualization with as little chart junk as possible and the largest data-to-ink ratio score imaginable?

Here, we will work with a simple data that has 2 columns. The first column is categorical and the second is quantitative. The data represents the frequency of letters, rounded, as they occur in a collection of English texts ([from wikipedia](https://en.wikipedia.org/wiki/Letter_frequency)). We will try to maximize our data-to-ink and visualize this as minimally as possible.

| Letter   | (%) |
| -------- | --- |
| a        |  8  |
| b        |  2  |
| c        |  3  |
| d        |  4  |
| e        |  13 |
| f        |  2  |
| g        |  2  |

A bar chart might be our first attempt to show this data:

<figure>
    <img src="https://www.frank.computer/images/minimalism1.png" alt="A bar chart of the previous data."/>
    <figcaption>A basic bar chart, already pretty minimal.</figcaption>
</figure>

So the bars technically have pixels, since this is a bitmap image. That means we can quantify our ink usage here. (For now, let's not count the pixels of our use of text.) So the bars have a hue encoding as well, so there is a second dimension encoded here. We will add up the pixels of all the bar heights (1081 pixels) and then multiply that by the width of the bars (70) and then again by 2 for using a color. We also have an axis line that is one pixel thick and 718 pixels wide, we will want to add that on to the previous total. So for now, we get a total "ink" value of 151340 + 718. Since data is a constant, we can set that to 1. Our **first design's data-to-ink ratio is 1:152058**.

So technically the hue here isn't adding anything. And the axis line is useless too. Plus, the contrast of the text is too high. (We aren't counting text here towards our ink score, but let's reduce that anyway.)

To fix this, let's use the lightest contrast colors for geometries (#949494) and text (#767676) that we can while still [passing accessibility standards](https://webaim.org/resources/contrastchecker/). (Technically, we still want to be "accessible" according to standards! We can't go too far in hue and lightness reduction...)

<figure>
    <img src="https://www.frank.computer/images/minimalism2.png" alt="A bar chart of the previous data, using grey bars and lighter text."/>
    <figcaption>A more minimal bar chart.</figcaption>
</figure>


Well, if we calculate this ratio for this one, it's much lower. The 718 from the axis line is gone and the hue is removed, so that extra dimension is gone. This one is **1:75670**; better but we can go a lot further. That is still far too much ink.

In Tufte's fashion, (I don't remember which book this is in) but we can acutally get rid of all the useless filling of the bars themselves and just leave the tops, marking the only part of their position that matters.

<figure>
    <img src="https://www.frank.computer/images/minimalism3.png" alt="A chart of the previous data, with light grey lines where the top of the bars used to be instead of bars."/>
    <figcaption>Our data:ink ratio is improving; who needs bars anyway?</figcaption>
</figure>

This chart is much better! Now we're much more minimal. So each of the 7 bars are only 5 pixels tall. That's 5 tall by 70 pixels wide by 7 marks total. Our data:ink ratio is skyrocketing now, at **1:2450**. We've gone down a whole order of magnitude!

But honestly, why did we stop there? Why waste all that ink making these bars so wide? We can take this design further.

<figure>
    <img src="https://www.frank.computer/images/minimalism4.png" alt="A chart of the previous data, with small squares where the top of the bars used to be instead of bars."/>
    <figcaption>Technically, the smallest marks possible make for the best visualizations - they waste as little ink as possible!</figcaption>
</figure>

Now each mark is only 5 pixels wide by 5 pixels tall. At 7 marks, that's a **data:ink ratio of 1:175**. We've gone down *another* order of magnitude!

Well some of you might be looking at this design and find it hard to perceive. Well guess what? That's what minimalism is all about! Technically, according to accessibility standards, there is no regulation for minimum sizes. This is not only a highly-efficient, chart-junk-free visualization, but it is also technically accessible! Amazing.

But yes, you guessed it: we can go even further.

Dear reader: are you familiar with what "[code golf](https://en.wikipedia.org/wiki/Code_golf)" is? It's a sport (of sorts) where people attempt to reduce the number of characters they use in source code in order to solve a problem. It tends to result in comically terse, virtually unreadable lines of code, but it still gets the job done. One of the best places to witness this recreational exercise is over on the [code golf stack exchange](https://codegolf.stackexchange.com/).

So what if we go to the *extreme* here with our data-to-ink ratio? What if we try to visualize our data using the smallest amout of ink possible?

For this dataset and using a modern, pixel-based display or rendering, I believe that this is the solution:

<figure>
    <img src="https://www.frank.computer/images/minimalism5.png" alt="A chart of the previous data, however it is imperceptably small, each data point is a single pixel and even the text has been made into a minimal number of pixels to match."/>
    <figcaption>Data-to-ink ratio meets code-golf, I call it "ink golf:" where you try to use the smallest amount of ink possible in order to maximize the data-to-ink ratio of a visualization.</figcaption>
</figure>

Each data point is represented by only a single pixel! For our dataset of 7 points, **this data:ink ratio is a massive 1:7**. This would surely make Edward Tufte happy! Obviously, this is the *pinnacle* of data visualization design!

## Minimalism has been a way for some "intellectuals" to enforce aesthetics as law
So while this exercise was meant as a playful exploration in my new sport, "ink golf," I do want to make the point that the graphic above is *obviously* inaccessible in its design.

Virtually nobody would find this design useful or effective and it is likely an unusable artifact. I am certain that Tufte wouldn't defend this design with any seriousness, and certainly wouldn't intend for his philosophies to be taken this far, either.

But yet, followers of minimalism always seem to stop at a certain point. Why? Why stop once you, the author of a visualization, are barely able to see what you've made? How do you know that what you see is adequate for what others see? Is *your* perception of minimalism the same as your audience's? Is minimalism, with so few real rules or empirically observed benefits, worth defending with such passion and fervor?

Minimalism becomes a barrier, if taken too far. And *this* is the question I want to raise: *when* is too far? When do we decide that minimalism is excluding people from using our data visualizations?

Accessibility standards don't save us. They currently don't set a minimum size for text or objects in a visualization.

We *do* have plenty of research on "[Just Noticeable Differences](https://ieeexplore.ieee.org/abstract/document/8017604?casa_token=3nllwCmAxi8AAAAA:kMy02ZIDga82EXJaYs1bcAeqgpEoYnrABVbBpWB0ns5sVPQvkY-y7SKGW0lIeAobY4k_q9mB)" or JNDs, however, but these aren't modeled after people with visual disabilities like low vision or blindness - so using these models wouldn't be helpful if we really wanted to know when minimalism starts to hit practical limits in design.

So my lesson for you, dear reader, is this: don't take minimalism so seriously. The data-to-ink ratio is not a law. And as Derya Akbaba says, perhaps [it is time to put the idea of "chart junk" in the trash](https://arxiv.org/abs/2109.10132) too.

<hr>
<br>
<br>

For fun, here is a zoomed in version of my *ink golf* solution, so you can see that I even custom-made a font in order to make this as small as possible. I reckon there might be some pixel configurations that can represent these letters in fewer pixels, but I couldn't solve it. I suppose that's the fun of golf - perhaps a lower score is possible! You're welcome to give it a try, as long as you remember that minimalism should be used for fun more than it is for any sort of deadly, professional *seriousness*.

<figure>
    <img src="https://www.frank.computer/images/data_to_ink.png" alt="A zoomed in version of the super small chart, showing that there really are only 7 pixels total for the data. The a is made with 5 pixels, b with 6, c with 3, d with 6, e with 6, f with 5, and g with 7."/>
    <figcaption>Yes, I even tried to do <i>ink golf</i> with the text. (Now that I think about it... maybe we can start using "ink golf" as a way to poke fun at those deadly-serious business intelligence utilitarians who seem to defend minimalsm with such fervor. They're just <i>ink-golfing enthusiasts</i>!)</figcaption>
</figure>

<hr>
<br>
<br>

## (May 12th) Addendum: responses to "ink golf" on social media

Well, I've had a blast over the last few weeks interacting with folks on social media with this. Folks on Linkedin, for the most part, still had fun. But some were very serious about my abuses and misrepresentations of Tufte's "theory" (in particular the caveat that the data-to-ink ratio is meant to be followed "within reason"). Ah, of course! If only I had read the holy text close enough. "Within reason" is so concrete, clear, and helpful! (In truth, knowing what the "reasons" are is, of course, most of the battle. This is why the data-to-ink ratio is a rough heuristic and not even remotely a real, working "theory" of any kind.)

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:jonnuvubyyf7xhsentiuyq3l/app.bsky.feed.post/3lniytgsyrk2v" data-bluesky-cid="bafyreieoh6j7hamhutzwzdhrjhs4iyeu4nby3drqyz46ysxu4summ5fydi" data-bluesky-embed-color-mode="system"><p lang="en">Linkedin is being very normal about this, by the way<br><br><a href="https://bsky.app/profile/did:plc:jonnuvubyyf7xhsentiuyq3l/post/3lniytgsyrk2v?ref_src=embed">[image or embed]</a></p>&mdash; Frank Elavsky ⌁ (<a href="https://bsky.app/profile/did:plc:jonnuvubyyf7xhsentiuyq3l?ref_src=embed">@frank.computer</a>) <a href="https://bsky.app/profile/did:plc:jonnuvubyyf7xhsentiuyq3l/post/3lniytgsyrk2v?ref_src=embed">April 23, 2025 at 4:10 PM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>


Bluesky has had a lot of fun by comparison, we even "ink golfed" just like folks do with code, incrementally iterating closer to various solutions together. Some favorites:

### First: text reduction

First, folks focused on reducing the pixels of the text. Of course, using English was short-sighted of me (pun intended). Turns out that braille-as-pixels is much more efficient:

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:gyf5jjsdx3fcjrosnn3p5mmy/app.bsky.feed.post/3lnidjdrzuk26" data-bluesky-cid="bafyreigngvjj3sisxg3x6hmtsowcvx2w2mkhp5p72qjyz66pucg7dtlkyi" data-bluesky-embed-color-mode="system"><p lang="en">if you&#x27;re gonna argue with minimalism, which is simply The Right Way, you should do it without standing up a straw man.

the optimal solution here is clearly using Braille for the column labels, which reduces the true data-ink ratio from a measly 1:45 (yours) to an impressive 1:24 (mine). &lt;/sarcasm&gt;<br><br><a href="https://bsky.app/profile/did:plc:gyf5jjsdx3fcjrosnn3p5mmy/post/3lnidjdrzuk26?ref_src=embed">[image or embed]</a></p>&mdash; István Korompai (<a href="https://bsky.app/profile/did:plc:gyf5jjsdx3fcjrosnn3p5mmy?ref_src=embed">@kpisti.bsky.social</a>) <a href="https://bsky.app/profile/did:plc:gyf5jjsdx3fcjrosnn3p5mmy/post/3lnidjdrzuk26?ref_src=embed">April 23, 2025 at 9:49 AM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

But if we don't need English, do we even need human language at all? What if we could mentally map letters to pixel positions? Reducing pixels is more important than anything, so this makes sense to explore.

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:c6b4jhahjjn75k4k2rvhsvyh/app.bsky.feed.post/3lnikbkfeb22k" data-bluesky-cid="bafyreihpfnaiiytbn5jdwkn4uzwjaqtyxbhzjlxtez2iu37hpm6m4nsvyq" data-bluesky-embed-color-mode="system"><p lang="en">The order of letters in the alphabet is set, so technically you don’t even need the labels.<br><br><a href="https://bsky.app/profile/did:plc:c6b4jhahjjn75k4k2rvhsvyh/post/3lnikbkfeb22k?ref_src=embed">[image or embed]</a></p>&mdash; Robert Simmon (<a href="https://bsky.app/profile/did:plc:c6b4jhahjjn75k4k2rvhsvyh?ref_src=embed">@rsimmon.bsky.social</a>) <a href="https://bsky.app/profile/did:plc:c6b4jhahjjn75k4k2rvhsvyh/post/3lnikbkfeb22k?ref_src=embed">April 23, 2025 at 11:50 AM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

A rather cerebral take in this direction:

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:2h5e6whhbk5vnnerqqoi256k/app.bsky.feed.post/3lnim4munuk2g" data-bluesky-cid="bafyreifvtkzdeuxjcl77ebmwrcvoaeei7ozxfz5ried7fmz7m6t6fc36dm" data-bluesky-embed-color-mode="system"><p lang="en">Cut the intermediate braille labels for even more information density! (people should of course be able to infer that the categories are in alphabetical order between a and g ;) )<br><br><a href="https://bsky.app/profile/did:plc:2h5e6whhbk5vnnerqqoi256k/post/3lnim4munuk2g?ref_src=embed">[image or embed]</a></p>&mdash; Randy Boyes (<a href="https://bsky.app/profile/did:plc:2h5e6whhbk5vnnerqqoi256k?ref_src=embed">@randy.pub</a>) <a href="https://bsky.app/profile/did:plc:2h5e6whhbk5vnnerqqoi256k/post/3lnim4munuk2g?ref_src=embed">April 23, 2025 at 12:23 PM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

### Reaching the QR-Code solution

From text reduction, two threads emerged. The first thread was on new and creative ways to encode the data into smaller spaces, specifically using a QR-code-like set of rules (the cropping is poor on these, clicking them shows how they work). Depending on your counting method, this uses 7 to 10 pixels for the data and the "text:"

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:wlwlvnq25nzwvz43crqo7apu/app.bsky.feed.post/3lningfgmk226" data-bluesky-cid="bafyreie76cepxokaccjwmizy4audf7ib2autyyopr5rf7atzhfsutgdlty" data-bluesky-embed-color-mode="system"><p lang="en">and if we do need exact precision, we can binary encode each square!

break each data point into 4 squares, color each subsquare black or white, then add up the black subsquares to get the value

extremely intuitive and user friendly<br><br><a href="https://bsky.app/profile/did:plc:wlwlvnq25nzwvz43crqo7apu/post/3lningfgmk226?ref_src=embed">[image or embed]</a></p>&mdash; shri (<a href="https://bsky.app/profile/did:plc:wlwlvnq25nzwvz43crqo7apu?ref_src=embed">@shrikhalpada.dev</a>) <a href="https://bsky.app/profile/did:plc:wlwlvnq25nzwvz43crqo7apu/post/3lningfgmk226?ref_src=embed">April 23, 2025 at 12:46 PM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

After discussion, the design became clearer:
<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:jonnuvubyyf7xhsentiuyq3l/app.bsky.feed.post/3lnitm3bjoc26" data-bluesky-cid="bafyreidvctorsqvv3iqmsabtabxqwsagcjz2sww72zug473y7npmtbruni" data-bluesky-embed-color-mode="system"><p lang="en">Lmao incredible. Basically interpreting a home-cooked QR code.</p>&mdash; Frank Elavsky ⌁ (<a href="https://bsky.app/profile/did:plc:jonnuvubyyf7xhsentiuyq3l?ref_src=embed">@frank.computer</a>) <a href="https://bsky.app/profile/did:plc:jonnuvubyyf7xhsentiuyq3l/post/3lnitm3bjoc26?ref_src=embed">April 23, 2025 at 2:37 PM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

My advisor, Dominik Moritz, remarked "you could probably put everything into a QR code, if it really is about efficiency." So, I reckon that this method scales well in theory.

### Reaching the best solution

But if it feels like "cheating" to turn data into a QR code (since that is mostly for machine interpretation), perhaps it makes sense to focus on human interpretation?

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:gyf5jjsdx3fcjrosnn3p5mmy/app.bsky.feed.post/3lnivre3dgs25" data-bluesky-cid="bafyreie6h5tnsn2ycz2sjthvtev3uahkro2btbsecftyyjeopb34tt2tfe" data-bluesky-embed-color-mode="system"><p lang="en">so, this is the final form?

I&#x27;d argue it&#x27;s truly minimal, we even managed to remove any morsel of meaning from it<br><br><a href="https://bsky.app/profile/did:plc:gyf5jjsdx3fcjrosnn3p5mmy/post/3lnivre3dgs25?ref_src=embed">[image or embed]</a></p>&mdash; István Korompai (<a href="https://bsky.app/profile/did:plc:gyf5jjsdx3fcjrosnn3p5mmy?ref_src=embed">@kpisti.bsky.social</a>) <a href="https://bsky.app/profile/did:plc:gyf5jjsdx3fcjrosnn3p5mmy/post/3lnivre3dgs25?ref_src=embed">April 23, 2025 at 3:16 PM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

This can be reduced, if we assume certain patterns:

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:2h5e6whhbk5vnnerqqoi256k/app.bsky.feed.post/3lniwd3zlmc2b" data-bluesky-cid="bafyreidhklkm5wuou3tcqs4clavjabamegssmu44i2smej3ll3u5xvbyom" data-bluesky-embed-color-mode="system"><p lang="en">You can cut one more pixel if you&#x27;re willing to assume you can interpolate to get blank points<br><br><a href="https://bsky.app/profile/did:plc:2h5e6whhbk5vnnerqqoi256k/post/3lniwd3zlmc2b?ref_src=embed">[image or embed]</a></p>&mdash; Randy Boyes (<a href="https://bsky.app/profile/did:plc:2h5e6whhbk5vnnerqqoi256k?ref_src=embed">@randy.pub</a>) <a href="https://bsky.app/profile/did:plc:2h5e6whhbk5vnnerqqoi256k/post/3lniwd3zlmc2b?ref_src=embed">April 23, 2025 at 3:25 PM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

And my final solution using 4 pixels, which I think is the best solution for this particular data (as long as we actually show pixels and focus on some human sort of rules for interpretation):

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:jonnuvubyyf7xhsentiuyq3l/app.bsky.feed.post/3lnix66i3ns2o" data-bluesky-cid="bafyreifxa5332wevplsurv6pqdchq626imjs4vmjnbih5wb4dye3se7c3e" data-bluesky-embed-color-mode="system"><p lang="en">Wait... I&#x27;ll do you one better. What if we follow your lead here but instead truncate the axis based on the lowest data value - it happens to be shared by 3. This means we can interpret any missing pixel along the x as the lowest value! This results in a 1:4 ratio for this dataset...<br><br><a href="https://bsky.app/profile/did:plc:jonnuvubyyf7xhsentiuyq3l/post/3lnix66i3ns2o?ref_src=embed">[image or embed]</a></p>&mdash; Frank Elavsky ⌁ (<a href="https://bsky.app/profile/did:plc:jonnuvubyyf7xhsentiuyq3l?ref_src=embed">@frank.computer</a>) <a href="https://bsky.app/profile/did:plc:jonnuvubyyf7xhsentiuyq3l/post/3lnix66i3ns2o?ref_src=embed">April 23, 2025 at 3:41 PM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

### The ultimate solution: visualize in your head

Of course, the immortal Eugene Wu took our methods to their logical extreme (in the true spirit of the sport of ink golf): to reduce ink as much as possible, the reader simply must read the data and then picture it in their head! This is, of course, the solution that scales the best to all other datasets and also requires no ink at all (unless "brain ink" is a thing?).

Bravo! The game has been won:

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:nhizaxkpcqfallaedhly7lwo/app.bsky.feed.post/3lnj25l4f4k2f" data-bluesky-cid="bafyreiftrduww2gl6bt4hvkfzca5eeimqfmmzrsidohvhhncxsgto6ntza" data-bluesky-embed-color-mode="system"><p lang="en">Since you are making assumptions about what the reader knows (axes, weird encodings), then if you also assume the reader is already familiar with the points, show an empty image.  1:0</p>&mdash; ewuuu (<a href="https://bsky.app/profile/did:plc:nhizaxkpcqfallaedhly7lwo?ref_src=embed">@eugenewu.net</a>) <a href="https://bsky.app/profile/did:plc:nhizaxkpcqfallaedhly7lwo/post/3lnj25l4f4k2f?ref_src=embed">April 23, 2025 at 4:34 PM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

<hr>
<br>
<br>

## Reflections
It is clear that the seriousness of something so loosely defined as a "data-to-ink ratio" still has a chokehold on the minds of business-y "thought leaders" in the large space of visualization. Tufte's "laws" really do rule the thoughts of ink-bros still, even when we show them data otherwise.

So I hope that this playful exploration has demonstrated that minimalism really is rather absurd.

### Understanding "ink"
For anyone interested in a rather lovely exploration of philosophy and ink, Tony Fast (a wonderful friend) recorded a stream reading this blog post while creating some art. [It was lovely](https://nbviewer.org/github/tonyfast/tonyfast/blob/main/tonyfast/xxiv/2025-04-24-stream.ipynb).

I do think that focusing on "ink" as a design heuristic is outdated. This mattered when strokes *had* to be precious, because there was also a cost of production and printing to keep in mind. Lighter, fewer marks made for cheaper prints.

### Further readings: minimalism and fascism
Ronke Babajide writes about how "[Minimalism is Rooted in Fascism](https://uxdesign.cc/how-minimalism-is-rooted-in-fascism-7204b15482a8)" in a great introduction to what I believe is one of the most important things to actually keep in mind when we critique minimalism. This blog was meant to be silly and absurd, to make a game out of minimalism. But as a tool, it has historically been [tied to white supremacy](https://title-mag.com/how-minimalism-and-white-supremacist-ideology-are-connected/), as Charlotte Eckardt writes.

Fascism, white supremacy, and minimalism are in my my mind as I watch the latest season of Andor:
<figure>
    <img src="https://www.frank.computer/images/isb.jpg" alt="14 officials sit around a round table, all of them human. Still image from Andor: the ISB meeting room, austere and geometric, bleach white. The room is stark contrast, almost entirely white with accents of pure black."/>
    <figcaption>The Empire loves minimalism. Look at this room of security officials: The room is as "pure" as it could be from blemishes and disorder; no wasted color, no aliens in sight, perfect geometric symmetry, clean, precise, and almost exclusively men. What better place to control the galaxy?</figcaption>
</figure>

Minimalism, especially with clean whiteness and obsessive control over any and all natural, organic characteristics, has strayed far from philosophies that focus on simple living, anti-consumerism, and humility.

I won't make the case that minimalisms in all forms are morally wrong, I certainly don't believe that; but I will argue that modern uses of minimalism-as-empire and minimalism-to-control-others are. Minimalism, especially in Tufte's data-to-ink ratio, can often become a tool to police the acts of others.

### Maximalism, decoration, and embellishment

I joked with Tony after he sent me his stream where he inked in response to my blog, that I'd love to see ink golf evolve into a game with very specific rules and counter-rules.

For example, perhaps it makes sense to create an outline around the "playing area" (a [magic circle](https://en.wikipedia.org/wiki/Magic_circle_(games)), if you will, for the game of ink golf). Whatever is inside the boundary is measured with intense scrutiny, as we demonstrated previously. But this would mean that, for the sake of *play*, whatever is outside of the bounds is fair game.

Perhaps a culture of [*itasha*](https://en.wikipedia.org/wiki/Itasha) would emerge, specific to ink-golfing (this is one of my favorite hyper-decorative subcultures). Or perhaps a specific counter-culture of [tag graffiti](https://en.wikipedia.org/wiki/Tag_%28graffiti%29) would become popular, where people would deface the outside area of *other* people's ink-golf submissions. My favorite example tag graffiti paradoxically respecting certain rules: [tag graffiti artists will avoid spraying over labels on trains](https://www.reddit.com/r/mildlyinteresting/comments/16yedk1/this_train_graffiti_artist_avoided_all_the_labels/), so that they either respect the safety/value that the labels accomplish *or* are just trying to maximize the chances that their tags don't get painted over.

So in an imagined hyper-culture of ink-golf, there might be some purists and some rebels, when it comes to rules-permitted decoration. My previous "solution" could instead look like this:

<figure>
    <img src="https://www.frank.computer/images/lemonalism.png" alt="My hyper-reduced solution that came from bluesky, but this time it has a black border around it. Outside of the border is an image of a sliced lemon pound cake."/>
    <figcaption>I love lemons and most things made with lemons. At IEEE VIS in 2023, I did a "lemonstration" of data navigator (where people could navigate a chart using lemons). I suppose this is some lemon-minimalism (or maximalism?). Anyway, it's <i>lemonalism</i>, either way.</figcaption>
</figure>

Plenty of good designs use a maximalist approach and I think they work quite well. For example, I play World of Warcraft with my wife. Many of the visualizations used by the websites tracking player data are quite maximal in their design:

<figure>
    <img src="https://www.frank.computer/images/class_distribution.png" alt="13 classes and 35 colors representing the specializations are organized in stacked bars. Each bar represents the distribution of all of the specializations at a given key level. There are a total of 19 bars shown, ranging from key levels +2 to 20."/>
    <figcaption>The "meta" in mythic+: A figure showing how 35 class and specialization distributions change as key levels get higher, from levels +2 to +20. "Keys" or "keystones" are a special type of dungeon (called "mythic+") that are unlocked with increasing levels of difficulty and must be completed in a set amount of time. "Dungeons" are a type of mini-game, so to speak, where a small team of 5 players (generally 1 healer, 1 tank, and 3 damage dealers) try to complete a non-random gauntlet of monsters and bosses. Higher and higher key levels end up filtering for only a few team compositions of specific class specializations. This visuaization shows what is called the "meta" of the game currently ("meta" meaning the best possible team you could have at this point in the game, according to the data). <a href="https://www.wowhead.com/news/holy-paladins-challenging-discipline-in-20s-tww-season-2-mythic-rankings-week-9-376766">Source: Wowhead</a></figcaption>
</figure>

But look at all of those colors! Of course, every color is meaningful and represents something in the data. It might appear to have noise, but it is mostly full of signal. Maybe this would [make the visualization minimalists happy](https://www.perceptualedge.com/blog/?p=2893)? Is 35 different categorical color encodings a good design choice? [Most recommend 5-7](https://www.sigmacomputing.com/blog/7-best-practices-for-using-color-in-data-visualizations), some even [recommend only 1 or 2 colors](https://www.datawrapper.de/blog/emphasize-with-color-in-data-visualizations) and use different methods than color for encoding (position, small multiples, etc). But I think this design choice is fine. It works well if you understand what the colors mean (they all map to a class specialization, which is a color scheme repeatedly used in-game). For this use, it's probably a totally acceptable design, despite breaking a zillion "rules" of visualization design.

But what is that *behind* the chart? There does seem to be some pesky decoration here... Let's look at a different chart to see this better:

<figure>
    <img src="https://www.frank.computer/images/key_level_run.png" alt="Bar chart showing the quantity of successful and failed dungeon runs ranging from +2 to +20."/>
    <figcaption>Distribution of mythic+ dungeons run at various keystone levels. This chart has the hero image used in the game's loading screen as a background for the visualization's data. (Also, as an aside: these charts were made with Highcharts! I love that the gaming community I am part of uses a chart library that I contributed a tiny bit of research towards.) <a href="https://www.wowhead.com/news/holy-paladins-challenging-discipline-in-20s-tww-season-2-mythic-rankings-week-9-376766">Source: Wowhead</a></figcaption>
</figure>

Uh oh! Now *this* is illegal embellishment, for sure!

I wonder what the earliest founders of data visualization would think about this? What would the progenitors and originators of our craft think? Let's check in with them:

<blockquote class="bluesky-embed" style="margin: 10px auto;" data-bluesky-uri="at://did:plc:nxtjxs4l37scbdun2i6jgon7/app.bsky.feed.post/3lnrbml4ks22w" data-bluesky-cid="bafyreihpit5nm3t5xkhke2agxp2mkegn6pkp4khcdp5bzvqm6lkf3hekoa" data-bluesky-embed-color-mode="system"><p lang="en">📊 I recently But found another pre-Playfair example, this by an unknown (to me) German, C.G. Porsch

&quot;Of the heights of the great watercourses of the Elbe River, near the town of Meiffen, Dresden, and the Electorate of Pilsen, from 1501 to 1784.&quot;

From: deutsche-digitale-bibliothek.de<br><br><a href="https://bsky.app/profile/did:plc:nxtjxs4l37scbdun2i6jgon7/post/3lnrbml4ks22w?ref_src=embed">[image or embed]</a></p>&mdash; Michael Friendly (<a href="https://bsky.app/profile/did:plc:nxtjxs4l37scbdun2i6jgon7?ref_src=embed">@datavisfriendly.bsky.social</a>) <a href="https://bsky.app/profile/did:plc:nxtjxs4l37scbdun2i6jgon7/post/3lnrbml4ks22w?ref_src=embed">April 26, 2025 at 11:09 PM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

In any case, there is quite a lot we still don't know about the use of decoration (or "embellishment") from a research perspective. Maybe some of these designs actually aren't that bad. Embellishments probably help make a visualization more memorable, they probably also really help with marketing and sharing (which is especially important for the success of truth). [Visualizations can be co-opted for evil](https://dl.acm.org/doi/abs/10.1145/3411764.3445211) as well as [leveraged for good](https://showyourstripes.info/).

So perhaps it is far more important for us, once we establish that we are visualizing towards honest ends, that we work to have an *impact* as well. Visualizations are often cultural artifacts, so they should participate in our cultures as well. The one thing we should really question in our designs is if minimalism's demand to strip ourselves of our cultural artifacts is worth it. Perhaps we *should* situate our designs more in the decorations and embellishments of our times, that matter to us.

> We might stand a chance in the war against dis- and misinformation if we could catch people's attention better than clickbait.

So the takeaway of this blog has now shifted from a joke poking fun at minimalism to a call to action: **use maximalism for good**. Catch people's attention, keep it, and make more memorable, meaningful visualizations.

