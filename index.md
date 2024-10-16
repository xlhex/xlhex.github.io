---
layout: page
title: About me
cover: false
---

I'm a Research Fellow at University College London ([NLP group](https://nlp.cs.ucl.ac.uk/)). I received my Ph.D. from Monash University (Australia), supervised by Prof. [Reza Haffari](http://users.monash.edu.au/~gholamrh/) and Dr. [Mohammad Norouzi](https://norouzi.github.io/). My recent research lies in an intersection between deep learning and natural language processing, with an emphasis on robustness and security in NLP models.

Now, I'm highlighting:
* Security and safety in NLP models
* Robustness in NLP models 

## Recent News
* \[September 2024 - Paper\]: Our paper “Generative Models are Self-Watermarked: Declaring Model Authentication through Re-Generation” is accpeted by TMLR 2024.
* \[August 2024 - Paper\]: I will be presenting a tutorial titled "A Copyright War: Authentication for Large Language Models" at IJCAI 2024.
* \[May 2024 - Paper\]: 2 papers accepted at ACL (1x)/ACL Findings (1x) 2024
* \[April 2024 - Paper\]: Our paper “SEEP: Training Dynamics Grounds Latent Representation Search for Mitigating Backdoor Poisoning Attacks” is accpeted by TACL 2024.
* \[March 2024 - Paper\]: 2 papers accepted at NAACL 2024

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

