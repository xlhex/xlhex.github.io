---
layout: page
title:  CV
cover:  false
menu:   true
order:  6
---

{% include cv-list.html categories=site.data.cv.before-pubs %}
<h2>Papers</h2>
{% include paper-list.html venue='journal' heading='Refereed journal articles' %}
{% include paper-list.html venue='conference' heading='Refereed conference papers' %}
{% include cv-list.html categories=site.data.cv.after-pubs %}


