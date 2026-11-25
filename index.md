---
layout: default
title: Home
---

# AI & Mathematics

<p class="lede"></p>

AI is changing math.
The goal of this site is to collect materials and resources for young researchers trying to decide how to use AI in their research.

<div class="mission" markdown="1">

**Core Principles**

- Researchers need to adapt to the new AI landscape
- We need to be dynamic, pragmatic, and strategic
- No one knows for sure what will happen in the next 3-5 years

</div>


For a general resource list on AI and math, check out [Northwestern's resource page](https://sites.northwestern.edu/airesourcesmath/).


## Opinions from Mathematicians

{% for q in site.data.quotes %}
<figure class="quote">
  <blockquote>{{ q.text | markdownify }}</blockquote>
  <figcaption>
    — {% if q.url %}<a href="{{ q.url }}">{{ q.who }}</a>{% else %}{{ q.who }}{% endif %}{% if q.source %}, <em>{{ q.source }}</em>{% endif %}
  </figcaption>
</figure>
{% endfor %}
