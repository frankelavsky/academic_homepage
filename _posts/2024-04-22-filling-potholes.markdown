---
layout: post
title: "Filling the potholes of the web."
slug: filling-potholes
tags:
- anarchism
- accessibility
- repair
- ambient co-presence
- cscw
description: People with the power to fix our inaccessible web have failed to do it for long enough. Isn't it time to imagine ways we can repair the web without waiting for them?
---
## What do we do when our digital infrastructures remain neglected?

Every single year I read the [WebAim Million](https://webaim.org/projects/million/) report and hope that real progress has been made. But sadly, 97 - 99% of the web's top 1 million home pages contain a critical accessibility failure that can be automatically detected. The web is really bad for people with disabilities and it has not gotten much better over the past 5 years since this large-scale survey started. I've even written about how [things are probably a whole lot worse that 99% inaccessible](https://www.frank.computer/blog/2022/03/facing-the-scale-of-digital-inaccessibility.html) too: only basic tests were run (not any of the harder or more complex issues), many issues can't be reliably caught with automated tests anyway (many false negatives), and only home pages were tested (which I assume are likely made more accessible than all the branching side-pages on any given website).

Unlike the web, in realspace communities can come together to take action to repair the world around them. In Portland, [anarchists took action and began filling potholes](https://www.bloomberg.com/news/articles/2017-03-15/portland-anarchist-road-care-fixes-potholes-anonymously) that the city had continued to neglect. While the anarchists had a minor impact in the scale of potholes they filled (they only claimed to have fixed 5 total), they [pressured municipal officials to host a "patch-a-thon"](https://www.portland.gov/transportation/news/2017/2/24/news-release-pbot-launches-patch-thon-address-potholes-caused-winter) that resulted in more than 1000 fixed potholes.

But in digital spaces, like on the web, we might "share" social media content with each other. However, we don't share the same material infrastructure in the same way realspace is shared. As the anarchists in Portland identified, ["coercive hierarchies" can often prevent direct action and repair in times of need](https://www.oregonlive.com/commuting/2017/03/why_portland_anarchists_are_pa.html).

If someone "repairs" a website, to make it more accessible for people with disabilities for example, those changes to the HTML, CSS, or JavaScript only persist for that person and during that session. If they reload their webpage, they get the same page infrastructure dished up to them from a server as everyone else would. All the labor of that repair is lost in an instant.

The web's technological infrastructure is governed by careful control of codebases, each managed and maintained by different organizations, communities, and companies. Even an "open source" website still regulates who can make changes to the code that lives on a server.

But if the current status quo of sociotechnical governance continues to fail people with disabilities - shouldn't it be time to fill the potholes of the web, like the Portland anarchists eventually did?

## My prototype and our group project

[My latest class project is a browser extension](https://github.com/frankelavsky/filling_potholes/) that explores the idea that edits and repairs to broken and inaccessible infrastructure can be shared across sessions and users, so long as they all share the same extension. This is just a prototype that uses static changes to a single website, so that we could get validation and feedback from folks with disabilities on the idea first.

The core idea for the project has been mine for a while now (a couple of years, in fact). But as a group, my collaborators have taken the idea even further, refining it and exploring it from different angles. Our big-picture goals involve keeping track of all of the changes made on a server, flagging issues for others to fix, intelligently managing identical assets such as alt text for the same images that might crop up in different locations, socially moderating and reviewing the changes made by others, automatically sending reports and github tickets to the owners of the original code being repaired, handling of multiple attempts at repair (such as different people authoring alt text for the same image), as well as a feedback system that people can give to other repairers and the codebase owners.

The technology used for this idea is inspired by two separate research projects: first is the idea of "[ambient co-presence](https://maggieappleton.com/ambient-copresence)." Here, we are exploring an *ambient co-repair*, where the vestiges and lingering traces of others aren't just ghostlike or aesthetic, but rather people leave their mark through the subtle and careful repair of the shared digital spaces we inhabit. The other idea is inspired by a project from CSCW where users had a browser extension and could [change the headlines on news articles to fix sensationalized and click-baity language](https://dl.acm.org/doi/10.1145/3555643) into something factual or more reasonable.

## Our case example and context: a really bad article on how "accessibility has failed"

I focused my repair on a single article by the now-infamous Jakob Nielsen that is ironically titled, ["Accessibility Has Failed: Try Generative UI = Individualized UX"](https://jakobnielsenphd.substack.com/p/accessibility-generative-ui). My fellow groupmate Julia brought the article to our group and it is a perfect example of a website with content that is sorely inaccessible.

<figure>
    <img src="https://www.frank.computer/images/failed.png" alt="Screenshot of Jakob Nielsen's article. VoiceOver screen reader is on a navbar icon of Jakob's face and the screen reader is announcing Unlabeled Image, Unlabeled Image."/>
    <figcaption>The very first element a screen reader accesses in the article for "Accessibility has failed" is a link that is unlabeled that contains an image without a description. Not a great start!</figcaption>
</figure>

The page has no alt text on any images, in the article and outside of the article (in images across the rest of the page). It also notably uses images as links (`<a>` elements), but they operate like `<button>` elements, and have no label, or ARIA information at all. To a blind person, this article would be a barren landscape.

Painfully, the article's main point is that large-language models might someday empower people with disabilities to build their own interfaces. If we use the metaphor of broken infrastructure, this would be like expecting wheelchair users in the 1970s to cut their own curbs. The assumption would then be that if demolition and construction equipment was cheap enough, surely wheelchair users would have the time, energy, and knowledge to cut the curbs that the city and legislators failed to.

The burden of repair, access, or "fit" being placed on people with disabilities is, and has been, a justice issue in technological innovation for a long time. I've [written about the issue of placing technical/system-related burdens](https://arxiv.org/pdf/2304.08748.pdf) on users with disabilities as well in one of my prior micro-papers. Ultimately, the people who built something broken should fix their own work.

## Feedback from blind people
I reached out to two blind folks I know, both of whom are fairly technical people (both have skills writing code and are familiar with modern advancements like LLMs and generative models). One is congenitally blind with no sight and the other has progressive blindness with partial remaining vision (very little acuity and about 10 degrees of visual field).

I showed them both the original article, watched them parse the page with their screen reader, and then we had a discussion about the piece.

After that, I had them install my extension and then parse the page again. We discussed the idea behind the extension and I got their thoughts and feedback.

Overall, my friends were relatively reserved and concerned with the practicality of the idea both socially and technically. The idea seemed good if enough people were involved and the stuff out there on the web lasted long enough.

One noted that changing a page is a good idea but "this probably won't scale well. What happens if the page updates something and the reference you have to the image changes? Or the owner uses the same page at a new link? Simple things like that might be hard to deal with." We would have have to build a really robust system to handle the relatively transient state of the web's core functionalities. Imagining constantly adding alt text to every new product image posted to Amazon, audio descriptions for every reel on instagram, or anything else related to the regular churn of the internet seemed unfeasible to them.

They also noted that the solutions added might come too late. They noted that viral pages, posts, and content get most of their traffic early on. But if nobody has flagged something as inaccessible or an issue and then a do-gooder doesn't respond in time, the opportunities to help people when they needed it could be mostly lost.

The other participant loved the idea and saw use for it in the context of web content that "tends to last longer than most social media." I followed up and asked for examples, they mentioned this could include things like articles, recipies, blog posts, knowledgebases, repositories, wikis, videos, and games. They also mentioned that reddit has a log of use over time compared to other social media sites, so repair would "make sense there because I still find myself on reddit posts more than a decade old regularly."

However this participant was primarily concerned with moderation issues. We had a lengthy discussion about how frustrating social spaces can be when people start using something like alt text "to voice opinions rather than just explain what something is." They mentioned that social media already has this problem even when people write their own alt text. And it could get worse if someone was able to essentially graffiti someone else's page (my choice of words here).

Despite their reservations, both participants expressed excitement at the possibility of using this anarchist approach to get companies and people in power to do the right thing. They mentioned that being able to automatically send complaints as well as a request for a fix would be really helpful. We also discussed the idea of having a third automatic communication channel to a disability lawyer who could begin to build a case for litigation, since historically that has been a significant moving force in the space of accessibility and is [gaining massive traction in recent years](https://www.forbes.com/sites/gusalexiou/2023/06/30/website-accessibility-lawsuits-rising-exponentially-in-2023-according-to-latest-data/?sh=6e86d0ef717f).

So perhaps the outcomes of this idea are similar to the Portland anarchists: the individual actions of repair may not be enough to solve the problems we have at scale, but it might just be enough to get the attention our broken digital world so desperately deserves.
