---
layout: page
permalink: /talks/
title: Talks
class: talks
---

<picture>
  <source srcset='/images/highsoft_talk' type='image/' />
  <img
    src='/images/highsoft_talk.png'
    alt="I'm standing in front of a screen, laughing. The screen says Looking to the future of accessible data interfaces.">
</picture>

# Talks, Workshops, and Guest Lectures

I am passionate about accessibility and data visualization, which is my most-common talk subject. (I love talking and teaching about other things too, of course.)

Below is one of my favorite talks, on *tool-making*, which I gave as the closing keynote for DDD Brisbane in December of 2025.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
  <iframe width="100%" height="100%" style="position: absolute; top: 0; left: 0;" src="https://www.youtube.com/embed/W9LDW-t09oY?si=fnWsKpKawhkwozmX&cc_lang_pref=en&cc_load_policy=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
<br>

{% assign talktitles = site.data.talks | group_by:"title" %}
{% for title in talktitles %}
{:.talk-title}
### {{ title.name }}
{% assign sorted_talks = title.items | sort: 'date' | reverse %}
{% for talk in sorted_talks  %}
  {% include talk.html talk=talk %}
{% endfor %}
{% endfor %}
