---
layout: default
title: Apps
permalink: /apps
---

# Software

<table>
  {% for software in site.software %}
    <tr>
      <td> <a href="{{ software.url }}">
        <div style="width:200px;height:200px">
          <img
            src="{{ software.image }}"
            style="width:100%;height:100%;object-fit:cover;display:block;" >
        </div>
      </a> </td>
      <td>
        <h2> <a href="{{ software.url }}"> {{ software.name }} </a> </h2>
        {{ software.short | markdownify }}
      </td>
    </tr>
  {% endfor %}
</table>

Discover more on my [Gitlab](https://gitlab.com/bous) page.
