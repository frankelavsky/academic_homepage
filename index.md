---
layout: page
title: "Home"
class: home
---

# Hi, I'm Frank Elavsky

<div class="columns" markdown="1">

<div class="intro" markdown="1">
I design and build <a href="https://www.frank.computer/projects/">systems</a> for human interaction. My current work is situated on toolmaking at the intersection of data visualization and accessibility. I'm interested in building tools for people who build interactive systems and ways that effective tool design can make data more accessible to everyone, starting with those historically excluded by poor system design: people with disabilities.

<!-- I build and research two kinds of tools that contribute to systems work: <i>frameworks</i>, as guides that help shape and generate the design of systems, and <i>building blocks</i>, as software and hardware resources that assist in framing and scaffolding work for system builders and maintainers. I <a href="https://www.frank.computer/projects/">build</a> using JavaScript, Python, C (arduino), fabrication, and a handful of other techniques. I do my <a href="https://www.frank.computer/papers/">research</a> through expert interviews, co-design, disability-centered design, disability-led design, and both qualitative and quantitative usability study methods. I'm interested in how "tools" (as I define them) shape human behavior and outcomes and how we can improve the way that we design and implement tools as well. -->

My work has been recognized for its <a href="https://hcii.cmu.edu/hcii-impacts/chartability">significant societal contributions</a>, shaping systems work in: 15+ government and policy orgs internationally (WHO, federal groups, and the European Commission), 40+ businesses and corporations (including 3 of the Fortune 5), 18+ news and journalism groups (BBC, NYT, Reuters, and more), 50+ community organizations and non-profits (Special Olympics, Data Visualization Society, arXiv), and 20+ higher-ed classrooms.

I personally haven't made millions of visualizations more accessible for people with disabilities. But my tools <i>have</i>. My work has enabled practitioners all over the world to improve the accessiblity of the systems <a>they</a> are building and maintaining. My mission is to continue to enable people to do informative, meaningful, and beautiful things using my tools.

I'm presently a PhD Candidate (ABD) at the [Human-Computer Interaction Institute](https://hcii.cmu.edu/) at [Carnegie Mellon University](https://www.cmu.edu/). I am advised by [Dominik Moritz](https://www.domoritz.de/) and [Patrick Carrington](https://www.patrickcarrington.com/) and a member of the [Data Interaction Group](https://dig.cmu.edu/) and [AXLE Lab](https://axle-lab.com/). I have had broad industry collaborations as well, with details you can find in [my cv](https://www.frank.computer/cv/).

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

## Why systems?
I create systems because <a href="https://www.frank.computer/blog/2024/11/love-of-systems.html">I love them</a>. I firmly believe that systems designed for rich human interactivity help us not only perform tasks but also enjoy what we are doing. And I have been creating systems for over two decades, starting with <a href="https://www.frank.computer/projects/#Personal:-Braven">designing rpg game systems</a> in middle school. Systems have been a way for me to playfully abstract difficult and complex problems as well as ground me concretely in real, tangible issues.

My Ph.D. dissertation, titled "<b>Toolmaking as an intervention on the accessibility of interactive data experiences</b>" (in progress) explores intellectual gaps at the intersection of data interaction and accessibility: "how can the design of tools (defined as a subtype of interactive system applied to a context), enable us to do entirely new things previously impossible, gain more confidence overcoming difficulty, reduce tedium in our work, and help people to actually enjoy interaction?"

## My background

<div class="intro" markdown="1">

Since starting my PhD, I have had collaborations with wonderful folks at [Highsoft's Highcharts](https://www.highcharts.com/) 📊, [Apple](https://www.apple.com/) <i class="fab fa-apple" aria-label="apple logo"></i>, [Adobe](https://www.adobe.com/), [Fizz Studio](https://fizz.studio/), [SRI](https://www.sri.com/research/education-learning/), [UW-Madison's WGNHS](https://home.wgnhs.wisc.edu/), [Northwestern University's MLDS](https://www.mccormick.northwestern.edu/machine-learning-data-science/), [Quansight Labs](https://labs.quansight.org/), [FiveThirtyEight](https://fivethirtyeight.com/), [tldraw](https://tldraw.dev/), [Visa](https://design.visa.com/data-visualization/charts/overview/examples/), and [Microsoft](https://www.microsoft.com/).

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
