---
layout: page
permalink: /blog/
title: Blog posts
---

# Being Frank on the Computer
There is very little quality assurance behind what goes in here, so keep that in mind. You can expect a mix of ranting and praise for things at the intersection of accessibility and data work, sometimes with other topics thrown in (aesthetics, epistemology, games, media, etc). I do plenty of navel-gazing, especially as it relates to research in Human-Computer Interaction. If you're into these sorts of things, welcome to my blog.

If you're curious about my shorter-form thoughts, follow me on my twitter account [@FrankElavsky](https://twitter.com/FrankElavsky), where I am regularly harping just the same as here but in slightly-smaller doses.

<!-- {% include search.html %} -->

<p class="rss-subscribe">Subscribe <a href="{{ "/feed.xml" | absolute_url }}">via RSS</a></p>

## Blog Posts

<div class="post-list">
  {% for post in site.posts %}
    {% assign currentdate = post.date | date: "%Y" %}
    {% if currentdate != date %}
      <h2 id="y{{ currentdate }}" class="year">{{ currentdate }}</h2>
      {% assign date = currentdate %}
    {% endif %}

    <div class="post-block">
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <span class="post-meta" title="{{ post.date | date: "%b %-d Y" }}">{{ post.date | date: "%b %-d" }} <span class="meta-year">{{ currentdate }}</span></span>
      {% if post.description %}<p class="post-subtitle">{{ post.description }}</p>{% endif %}
    </div>
  {% endfor %}
</div>

## Good Twitter Threads I've Written
A self-sommelier of sorts, selecting my favorite threads. (I love that [Crystal Lee did this on her blog](https://crystaljjlee.com/index/), so I am following suit!)

<div class="post-list twitter-posts">
  {% for post in site.data.threads %}
    {% assign currentdate = post.date | date: "%Y" %}
    {% if currentdate != date %}
      {% assign date = currentdate %}
    {% endif %}

    <div class="post-block">
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span class="post-meta" title="{{ post.date | date: "%b %-d %Y" }}">{{ post.date | date: "%Y, %b %-d" }}</span>
    </div>
  {% endfor %}
</div>