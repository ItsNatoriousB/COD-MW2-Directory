---
date: 2020-11-20 21:00:00
layout: weapon-post
datatable: true
title: BOCW Weapons
subtitle: "xModel names for weapons"
description: >-
  "xModel list for gun names"
image: >-
  https://res.cloudinary.com/natoriousb/image/upload/v1605925653/headers/Multiplayer_Screenshot_12_jct9fr.jpg
optimized_image: >- 
  https://res.cloudinary.com/natoriousb/image/upload/v1605925653/headers/Multiplayer_Screenshot_12_jct9fr.jpg
featured_image: >-
  https://res.cloudinary.com/natoriousb/image/upload/v1605925653/headers/Multiplayer_Screenshot_12_jct9fr.jpg
category: assets
tags:
  - weapons
  - hashes
  - names
author: itsnatorioub
paginate: true
credits:
  - Scobalula
  - DTZxPorter
  - Activision
  - Infinity Ward
  - Raven
  - High Moon
version: v1.0.0.0
game: "Call of Duty: Black Ops Cold War (2020)"
type: custom_content
---

<div class="datatable-begin row-border stripe"></div>
<table class="weapons-table display">
  {% for row in site.data.weapons %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {%- endfor -%}
    </tr>
    {% endif %}

   {% tablerow pair in row %}
   {{ pair[1] }}
   {% endtablerow %}
  {%- endfor -%}
</table>
<div class="datatable-end"></div>