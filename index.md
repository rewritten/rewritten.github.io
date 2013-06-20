---
layout: default
title: Rewritten
---
<h1>Rewritten's <tt>whoami</tt></h1>
<pre>saverio.trioni  tty??    May 20 07:22   .        394  term=0 exit=0</pre>


<div class="container">
  <div class="row">
    <div class="span4 links">
      <h3>profiles</h3>
      <ul>
        <li><a href="http://www.linkedin.com/in/saveriotrioni">LinkedIn</a></li>
        <li><a href="https://github.com/rewritten">GitHub</a></li>
        <li><a href="http://stackoverflow.com/users/384417/rewritten">StackOverflow</a></li>
        <li><a href="https://www.facebook.com/saveriotrioni">Facebook</a></li>
        <li><a href="http://www.flickr.com/people/saverio/‎">Flickr</a></li>
        <li><a href="https://plus.google.com/116362878025063680326" data-icon="google-plus">Google +</a></li>
        <li><a href="http://pinterest.com/rewritten2013/">Pinterest</a></li>
      </ul>

    </div>
    <div class="span4 about">

    </div>
    <div class="span4 gigs">
      <h3>gigs</h3>
      {% for page_in_order in site.pages %}
        {% if page_in_order.categories contains 'gig' %}
          <h4><a href="{{ page_in_order.url }}">{{ page_in_order.title }}</a></h4>
          <p>{{ page_in_order.lead }}</p>
        {% endif %}
      {% endfor %}

    </div>
  </div>
</div>
