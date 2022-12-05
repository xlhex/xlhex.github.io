---
layout: page
title: About me
cover: false
---

I'm a Research Fellow at University College London ([NLP group](https://nlp.cs.ucl.ac.uk/)). I received my Ph.D. from Monash University (Australia), advised by be supervised by Prof. [Reza Haffari](http://users.monash.edu.au/~gholamrh/) and Dr. [Mohammad Norouzi](https://norouzi.github.io/). My recent research lies in an intersection between deep learning and natural language processing, with an emphasis on robustness and security in NLP models.

Now, I'm highlighting:
* Security in NLP models, including privacy leakage and protection, backdoor attack and defense, imitation attack and defense
* Robustness in NLP models 

## Recent News
* I joined UCL as a Research Fellow under the supervision of Dr. [Pontus Stenetorp](https://pontus.stenetorp.se/) and Dr. [Pasquale Minervini](http://www.neuralnoise.com/)
* I did my internship at Amazon Search (Seattle, WA) (Jul-Oct, 2021)
* I did my internship at Adobe Research (San Jose, CA) (Jul-Sep, 2019)

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

