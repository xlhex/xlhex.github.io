---
layout: page
title: About me
cover: false
---

I'm a second year PhD student at Monash University (Australia). It's my honour to
be supervised by Prof. [Reza Haffari](http://users.monash.edu.au/~gholamrh/)
and Dr. [Mohammad Norouzi](https://norouzi.github.io/). I'm primarily working
on sentence generation, specifically with machine translation. Machine translation
is a challenging and exciting topic in Natural Language Processing (NLP) field,
which tries to teach machines to automatically translate one language to
another language(s).

Now, I'm highlighting:
* Translation with diversity, *i.e.* generating multiple correct translations for
a given source sentence

## Recent News
* I did my internship at Imagination Lab, Adobe Research with [Quan Tran](https://research.adobe.com/person/quan-hung-tran/), [Trung Bui](https://research.adobe.com/person/trung-bui/), [Walter Chang](https://research.adobe.com/person/walter-chang/), and [Zhe Lin](https://research.adobe.com/person/zhe-lin/) (Jul-Sep, 2019)

## Recent Research Highlights

<ul>
{% for paper in site.data.papers.papers %}
  {% if paper.selected %}
  <li>
  {% include paper.html paper=paper %}
  </li>
  {% endif %}
{% endfor %}
</ul>

