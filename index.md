---
layout: page
title: "Home"
class: home
---

# Hi, I'm Frank Elavsky

<div class="columns" markdown="1">

<div class="intro" markdown="1">

I design and build software <strong><a href="https://www.frank.computer/projects/">systems</a> for human interaction</strong>. My current work is situated on <strong>toolmaking</strong> at the intersection of data <strong>visualization and accessibility</strong>, making better frameworks and software tools for practitioners to make data visualizations accessible for people with disabilities. I hope to continue to design and build interfaces, infrastructures, and tools that <strong>enable everyone, including people with disabilities</strong>, to live full lives.

My work has been recognized for its <a href="https://hcii.cmu.edu/hcii-impacts/chartability">significant societal contributions</a>, shaping systems work in: 15+ government and policy orgs internationally (World Health Organization, European Commission), 80+ businesses and corporations (including 3 of the Fortune 5), 20+ news and journalism groups (BBC, NYT), 50+ community organizations and non-profits (Special Olympics, Data Viz Society), and 24+ higher-ed classrooms.

In the Fall of 2026, I will be an incoming assistant professor of data science at [Cal Poly](https://www.calpoly.edu/), in San Luis Obispo. I'm presently a PhD Candidate (ABD) at the [Human-Computer Interaction Institute](https://hcii.cmu.edu/) at [Carnegie Mellon University](https://www.cmu.edu/). I am advised by [Dominik Moritz](https://www.domoritz.de/) and [Patrick Carrington](https://www.patrickcarrington.com/) and a member of the [Data Interaction Group](https://dig.cmu.edu/) and [AXLE Lab](https://axle-lab.com/). I have had broad industry collaborations as well, with details you can find in [my cv](https://www.frank.computer/cv/).

</div>

<div class="me" markdown="1">
<picture>
  <source srcset='/images/headshot.jpg' type='image/jpg' />
  <img
    src='/images/headshot.jpg'
    alt="It's me! A white man smiling in a sunlit alleyway with medium-short brown hair, seaglass green trimmed glasses, and a tan overcoat.">
</picture>

{:.no-list}
* Incoming:
* Assistant Prof of Data Science
* Cal Poly
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

<!-- ## What's next?

<p>My <strong>5-year vision</strong> after the completion of my PhD thesis continues my focus on tools as an intervention on human behavior. However, I will be integrating critical concerns for broader impacts of technical tools on society and our lived environments. My research agenda has three pillars: <i>creation</i>, <i>critique</i>, and <i>care</i>:
</p>
<ol>
  <li><i>On creation:</i> I will contribute <b>practical advancements</b> in the state of the art in accessible data visualization tool development. I have made a career of building and co-designing useful tools that find purchase in working communities. I will strengthen this work moving forward, focusing especially on making accessibility work more accessible and scaling accessibility infrastructure.</li>
  <li><i>On critique:</i> I will contribute <b>humanistic and critical inquiry</b> of tools and toolmaking, within the social context of disability. My agenda will not solely focus on optimistic production of technology, but also advance our understanding of the past harms, present limitations, and future challenges of the sociotechnical entanglement of tools and the construct of disability.</li>
  <li><i>On care:</i> I will contribute <b>theoretical and empirical knowledge</b> of practitioner-tool relationships. I intend to investigate why tool-users and tool makers choose to care for, and not care for, some tools. On <i>caring for</i>, I will conduct longitudinal interview, co-design, and ethnographic work in the context of open-source software maintenance, specifically focusing on contexts of accessibility repair. On <i>not-caring for</i>, I intend to investigate, through qualitative expert interviews, preliminary research into why some practitioners respond to generative and agentic AI with disgust and refusal.</li>
</ol> -->

<!-- ## Why systems?
I create systems because <a href="https://www.frank.computer/blog/2024/11/love-of-systems.html">I love them</a>. I firmly believe that systems designed for rich human interactivity help us not only perform tasks but also enjoy what we are doing. And I have been creating systems for over two decades, starting with <a href="https://www.frank.computer/projects/#Personal:-Braven">designing rpg game systems</a> in middle school. Systems have been a way for me to playfully abstract difficult and complex problems as well as ground me concretely in real, tangible issues.

My Ph.D. dissertation, titled "<b>Toolmaking as an intervention on the accessibility of interactive data experiences</b>" (in progress) explores intellectual gaps at the intersection of data interaction and accessibility: "how can the design of tools (defined as a subtype of interactive system applied to a context), enable us to do entirely new things previously impossible, gain more confidence overcoming difficulty, reduce tedium in our work, and help people to actually enjoy interaction?" -->

## My background

<div class="intro" markdown="1">

During my PhD, I had collaborations with wonderful folks at [Highsoft's Highcharts](https://www.highcharts.com/) 📊, [Apple](https://www.apple.com/) <i class="fab fa-apple" aria-label="apple logo"></i>, [Adobe](https://www.adobe.com/), [Fizz Studio](https://fizz.studio/), [SRI](https://www.sri.com/research/education-learning/), [UW-Madison's WGNHS](https://home.wgnhs.wisc.edu/), [Northwestern University's MLDS](https://www.mccormick.northwestern.edu/machine-learning-data-science/), [Quansight Labs](https://labs.quansight.org/), [FiveThirtyEight](https://fivethirtyeight.com/), [tldraw](https://tldraw.dev/), [Visa](https://design.visa.com/data-visualization/charts/overview/examples/), and [Microsoft](https://www.microsoft.com/).

I was formerly a [W3C invited expert in data visualization in the ARIA Working Group](https://www.w3.org/groups/wg/aria/former-participants/#:~:text=Frank%20Elavsky) and currently still volunteer my time with [other efforts](https://www.frank.computer/cv/#service).

Before embarking on a PhD I was a staff design systems engineer at Visa on their Data Experience team and lead contributor to the accessibility efforts of their first open source library, [Visa Chart Components](https://github.com/visa/visa-chart-components). We were able to do some pretty extraordinary things together and I am fortunate to have worked alongside such world-class folks.

Prior to Visa I had a high-octane 2 years at Northwestern University working for Research Computing Services providing data visualization support to over two dozen research projects across a wide range of disciplines. Several of my projects [won awards](https://www.frank.computer/cv/#awards) and have been featured in over 60 research publications (including the privilege of being uncredited in the [2017 Nobel Lecture on Physics](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.90.040502)), 100+ web articles, 4 PhD theses, 4 graduate courses, and [9 textbooks](https://www.google.com/search?q=%22Frank+elavsky%22&hl=en&tbm=bks&sxsrf=APq-WBuA3-rFi5BAWgvu7rf_ax78Iee66w:1648824562316&ei=8hBHYsf-Eu-FytMPsZ-B0AI&start=0&sa=N&ved=2ahUKEwjHv9WSjvP2AhXvgnIEHbFPACo4ChDy0wN6BAgBED0&biw=896&bih=931&dpr=2).

In my early career (before Northwestern), I worked in federal policy analyzing large, complex medicare/medicaid datasets and building visualization tools for lawyers and policymakers.

And before I had a "career" in any singular sense (which I embarked on when I graduated undergrad in 2016), I worked many different jobs since as far back as age 7 (with only 1 gap where I wasn't working at least some job on the side or sick from disability). Most of these are part-time, overlapping, and off and on; they're listed in reverse chronological order based on the last time I did that job: **institutional research intern** (1yr), **barista** (9yrs), **community organizer** (3yrs), **night security** (2yrs), **editor** (1.5yrs), **Greek and English tutor** (2yrs), professional and volunteer **youth worker** (4yrs), **assistant manager** of a pottery/fused glass workshop (2yrs), **toy store clerk** (2yrs), **small business owner** (2yrs), **carpenter** and residential **painter** (3yrs), **furniture mover** (2yrs), **commissioned artist** (0.5yrs), **pizza maker** (1.5yrs), **doughboy** and **dishrat** (2yrs), **confectioner's apprentice** (1.5yrs), and **paperboy** (7yrs).

I won "paperboy of the quarter" in Q1 of 2004 and subsequently quit the following quarter. I still have the plaque! My mom first got me that job (initially under her name, since employing a 7 year old is definitely against child labor laws). She was very pro- when it came to child labor. There were about 1.5 years between age 14 (in '04) and my first wage job at 15.5 where I didn't have any job. Consequently, that was also the time I assembled my first coherent draft of [Braven](https://www.frank.computer/projects/#Personal:-Braven), which I had started working on in '02 (and still work on, to this day).

Despite all of this, I am definitely anti- "hustle culture." 7 year olds shouldn't be delivering papers. And when I wasn't working for that tiny window in my childhood, I gave life to my favorite, longest running hobby: writing fiction. I look forward to many future nights, weekends, and years of my life where I'm not laboring quite as much. All the bet things I've done in my life, didn't make any money at all.

</div>

<div class="news-travel" markdown="1">

<div class="news" markdown="1">
## Latest News

<ul>
{% for news in site.data.news limit:6 %}
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
