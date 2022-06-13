---
layout: page
title: Transcripciones
permalink: /transcripciones/
---

<table class="py-2 mb-4">
        <tr>
        <th>Lengua</th>
        <th>Palabras</th>
        <th>Duración (min)</th>
        <th>Fuentes</th>
      </tr>
      {% for row in site.data.totales_audio %}
      <tr>
        <td>{{ row.Lengua }}</td>
        <td>{{row.Palabras}}</td>
        <td>{{row.Dur}}</td>
        <td>{{row.Fuentes}}</td>
      </tr> 
      {% endfor %}
</table>