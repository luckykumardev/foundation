---
layout: default
order: 1
title: Team
permalink: /team/
---

<h1>The Oppia Foundation Team</h1>
<h2>Oppia is powered by volunteers from across the globe.</h2>
<p>Oppia's open source community consists of learners, educators, and technologists from all walks of life. Our contributors include people who have worked for leading companies like Google, Quora, and Codecademy, and have attended renowned institutions like Stanford, Carnegie Mellon, and the University of Cambridge. Though our community is incredibly diverse, all of our contributors share the same commitment to improving the quality of education around the world.</p>

<div class="card-container">
{% for person in site.data.team %}
  <div class="person-card">
    <div class="person-card-header">
      <img src="{{ site.baseurl }}/images/{{ person.image }}" />
      <h3>{{ person.name }}</h3>
      <h4>{{ person.role }}</h4>
    </div>
    <p>{{ person.bio }}</p>
  </div>
{% endfor %}

  <div class="person-card">
    <div class="person-card-header">
      <img src="{{ site.baseurl }}/images/you.png" />
      <h3>You?</h3>
      <h4>Generous Contributor</h4>
    </div>
    <p>Oppia is a community project, and we wouldn't be able to help so many learners without the support of our many generous contributors. These educators, technologists, and philanthropists have a massive impact on our ability to reach more learners, and we think <em>you</em> could make a significant difference too. <a class="inline-cta" href="{{ site.baseurl }}/get-involved/">Click here to see how you can help.</a></p>
  </div>
</div>
