---
layout: default
title: Home
---

# AI & Mathematics

<p class="lede">AI tools are changing how mathematical research is done. This site collects writing, organizations and resources to help mathematicians respond.</p>

<div class="mission" markdown="1">

**Our mission**

- Researchers need to adapt to the new AI landscape.
- We need to be dynamic, pragmatic, and strategic.
- We need to own our narrative, instead of letting others write it for us.

</div>

See the [Resources]({{ '/resources/' | relative_url }}) tab for articles, organizations, declarations and more.

## In their words

{% for q in site.data.quotes %}
<figure class="quote">
  <blockquote>{{ q.text | markdownify }}</blockquote>
  <figcaption>
    — {% if q.url %}<a href="{{ q.url }}">{{ q.who }}</a>{% else %}{{ q.who }}{% endif %}{% if q.source %}, <em>{{ q.source }}</em>{% endif %}
  </figcaption>
</figure>
{% endfor %}
