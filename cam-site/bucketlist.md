---
layout: page
permalink: /bucketlist/
title: My Bucket List
---


<div class="bucketlist">
  {% for category in site.data.bucketlist %}
  <h2>{{ category.category }}</h2>
  {% for item in category.items %}
  <div class="list-item">
    <h4 class="item">{{ item.name }}</h4>
    <h4 class="status {% if item.status == 'Not Started' %}status-not-started{% elsif item.status == 'Complete' %}status-complete{% else %}status-in-progress{% endif %}">{{ item.status }}</h4>
  </div>
  {% endfor %}
  {% endfor %}
</div>




