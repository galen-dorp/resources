---
layout: default
title: Home
---

# Ghost in the Shell

<p class="lede"></p>

AI is changing math.
Researchers need to adapt, especially early-career researchers.
Our goal is to help help young researchers decide for themselves how they want to interact with AI.

For a general resource list on AI and math, check out [Northwestern's resource page](https://sites.northwestern.edu/airesourcesmath/).

<div class="mission" markdown="1">

**Our Hypotheses**

- Researchers need to adapt to the new AI landscape
- We need to be dynamic, pragmatic, and strategic
- No one knows for sure what will happen in the next 3-5 years

</div>





## Opinions from Mathematicians

{% for q in site.data.quotes %}
<figure class="quote">
  <blockquote>{{ q.text | markdownify }}</blockquote>
  <figcaption>
    — {% if q.url %}<a href="{{ q.url }}">{{ q.who }}</a>{% else %}{{ q.who }}{% endif %}{% if q.source %}, <em>{{ q.source }}</em>{% endif %}
  </figcaption>
</figure>
{% endfor %}
