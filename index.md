---
layout: page
title: "Home"
class: home
---

# Hi, I'm Frank Elavsky

<div class="columns" markdown="1">

<div class="intro" markdown="1">
I research, design, engineer, contribute to standards, and talk about things at the intersection of data work and accessibility. I consider myself a maker and a builder before anything else, but I like to think I also do this work critically.

I'm a PhD student and researcher at the [Human-Computer Interaction Institute](https://hcii.cmu.edu/) at [Carnegie Mellon University](https://www.cmu.edu/). I am advised by [Dominik Moritz](https://www.domoritz.de/) and [Patrick Carrington](https://www.patrickcarrington.com/) and a member of the [Data Interaction Group](https://dig.cmu.edu/) and [AXLE Lab](https://axle-lab.com/).

I also offer part-time consulting services on a case by case basis, from single-session calls to large, on-going projects. My more recent work (both big and small) includes collaboration with the wonderful folks at [Highsoft's Highcharts](https://www.highcharts.com/) 📊, [Apple](https://www.apple.com/) <i class="fab fa-apple"></i>, [Adobe](https://www.adobe.com/), [Fizz Studio](https://fizz.studio/), [SRI](https://www.sri.com/research/education-learning/), [UW-Madison's WGNHS](https://home.wgnhs.wisc.edu/), [Northwestern University's MLDS](https://www.mccormick.northwestern.edu/machine-learning-data-science/), [Quansight Labs](https://labs.quansight.org/), [FiveThirtyEight](https://fivethirtyeight.com/), [tldraw](https://tldraw.dev/), and [Microsoft](https://www.microsoft.com/). As of Jan 2024: I am likely booked for larger projects until the end of the summer of 2026. Please don't hestitate to reach out, I would still be happy to discuss what you're up to, connect you to folks, and send over resources.

</div>

<div class="me" markdown="1">
<picture>
  <source srcset='/images/frank.jpg' type='image/jpg' />
  <img
    src='/images/frank.jpg'
    alt="It's me! A white man smiling with medium-short brown hair, glasses, and a grey t-shirt.">
</picture>

{:.no-list}
* <a href="mailto:{{ site.email }}">{{ site.email }}</a>
* {{ site.address }}
</div>

</div>

## Featured <a href="{{ "/projects/" | relative_url }}">Projects</a>

<div class="featured-projects">
  {% assign sorted_projects = site.data.projects | sort: 'highlight' %}
  {% for project in sorted_projects %}
    {% if project.highlight %}
      {% include project.html project=project %}
    {% endif %}
  {% endfor %}
</div>
<a href="{{ "/projects/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show More Projects
</a>

## Featured <a href="{{ "/publications/" | relative_url }}">Publications</a>

<div class="featured-publications">
  {% assign sorted_publications = site.publications | sort: 'year' | reverse %}
  {% for pub in sorted_publications %}
    {% if pub.highlight %}
      <a href="{{ pub.html }}" class="publication">
        <strong>{{ pub.title }}</strong>
        <span class="authors">{% for author in pub.authors %}{{ author }}{% unless forloop.last %}, {% endunless %}{% endfor %}</span>.
        <i>{% if pub.venue %}{{ pub.venue }}, {% endif %}{{ pub.year }}</i>.
        {% for award in pub.awards %}<br/><span class="award"><i class="fas fa-{% if award == "Best Paper Award" %}trophy{% else %}award{% endif %}" aria-hidden="true"></i> {{ award }}</span>{% endfor %}
      </a>
    {% endif %}
  {% endfor %}
</div>

<a href="{{ "/publications/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show All Publications
</a>

## My background

<div class="intro" markdown="1">

I was formerly a [W3C invited expert in data visualization in the ARIA Working Group](https://www.w3.org/groups/wg/aria/former-participants/#:~:text=Frank%20Elavsky) and currently still volunteer my time with [other efforts](https://www.frank.computer/cv/#service).

Before embarking on a PhD I was a staff design systems engineer at Visa on their Data Experience team and lead contributor to the accessibility efforts of their first open source library, [Visa Chart Components](https://github.com/visa/visa-chart-components). We were able to do some pretty extraordinary things together and I am fortunate to have worked alongside such world-class folks.

Prior to Visa I had a high-octane 2 years at Northwestern University working for Research Computing Services providing data visualization support to over two dozen research projects across a wide range of disciplines. Several of my projects [won awards](https://www.frank.computer/cv/#awards) and have been featured in over 60 research publications (including the privilege of being uncredited in the [2017 Nobel Lecture on Physics](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.90.040502)), 100+ web articles, 4 PhD theses, 4 graduate courses, and [9 textbooks](https://www.google.com/search?q=%22Frank+elavsky%22&hl=en&tbm=bks&sxsrf=APq-WBuA3-rFi5BAWgvu7rf_ax78Iee66w:1648824562316&ei=8hBHYsf-Eu-FytMPsZ-B0AI&start=0&sa=N&ved=2ahUKEwjHv9WSjvP2AhXvgnIEHbFPACo4ChDy0wN6BAgBED0&biw=896&bih=931&dpr=2).

In my early career (before Northwestern), I worked in federal policy analyzing large, complex medicare/medicaid datasets and building visualization tools for lawyers and policymakers.

</div>

<div class="news-travel" markdown="1">

<div class="news" markdown="1">
## Latest News

<ul>
{% for news in site.data.news limit:10 %}
  {% include news.html news=news %}
{% endfor %}
</ul>

</div>

<div class="travel" markdown="1">
## Latest Visits

<table>
<tbody>
{% assign future_travel = site.data.travel | where_exp:'item','item.start == null' %}
{% for travel in future_travel %}
  {% include travel.html travel=travel %}
{% endfor %}
{% assign sorted_travel = site.data.travel | where_exp:'item','item.start' | sort: 'start' | reverse %}
{% for travel in sorted_travel limit:10 %}
  {% include travel.html travel=travel %}
{% endfor %}
</tbody>
</table>

</div>

</div>
