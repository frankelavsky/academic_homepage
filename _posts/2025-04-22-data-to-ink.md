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

For fun, here is a zoomed in version of my *ink golf* solution, so you can see that I even custom-made a font in order to make this as small as possible. I reckon there might be some pixel configurations that can represent these letters in fewer pixels, but I couldn't solve it. I suppose that's the fun of golf - perhaps a lower score is possible! You're welcome to give it a try, as long as you remember that minimalism should be used for fun more than it is for any sort of deadly, professional *seriousness*.

<figure>
    <img src="https://www.frank.computer/images/data_to_ink.png" alt="A zoomed in version of the super small chart, showing that there really are only 7 pixels total for the data. The a is made with 5 pixels, b with 6, c with 3, d with 6, e with 6, f with 5, and g with 7."/>
    <figcaption>Yes, I even tried to do *ink golf* with the text.</figcaption>
</figure>
