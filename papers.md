---
layout: page
title:  Papers
cover:  false
menu:   true
order:  1
---

> _Research is an organized method of trying to find out what you are
> going to do after you cannot do what you are doing now. It may also
> be said to be the method of keeping a customer reasonably dissatisfied
> with what he has. That means constant improvement and change so that
> the customer will be stimulated to desire the new product enough to buy
> it to replace the one he has._
>
> ---Charles F. Kettering

<ul>
{% for paper in site.data.papers.papers %}
  <li>
  {% include paper.html paper=paper %}
  </li>
{% endfor %}
</ul>

