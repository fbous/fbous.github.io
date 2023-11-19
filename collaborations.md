---
layout: default
title: Collaborations
permalink: /collaborations
---

# Collaborations with artists

<table>
  {% assign sorted = site.collaborations | sort: "year" %}
  {% for collaboration in sorted reversed %}
    <tr>
      <td> <a href="{{ collaboration.url }}">
        <div style="width:150px;height:150px">
          <img
            src="{{ collaboration.image }}"
            style="width:100%;height:100%;object-fit:cover;display:block;" >
        </div>
      </a> </td>
      <td>
        <h2> <a href="{{ collaboration.url }}">
          {{ collaboration.name }}
          {% if collaboration.year %}
            ({{ collaboration.year }})
          {% endif %}
        </a> </h2>
        <i> {{ collaboration.type }} </i>
        {{ collaboration.short | markdownify}}
      </td>
    </tr>
  {% endfor %}
</table>
