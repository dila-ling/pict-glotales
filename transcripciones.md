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

<!--table id="table_id" class="display table py-2 mb-4">
  <thead>
    <tr><th class="th-sm">Lengua</th><th class="th-sm">Palabras</th><th>Duración (min)</th><th>Fuentes</th></tr>
  </thead>
  <tbody>
  {% for row in site.data.totales_audio %}
      <tr><td>{{ row.Lengua }}</td><td class="italic">{{ row.Palabras }}</td><td class="italic">{{ row.Dur }}</td><td class="italic">{{ row.Fuentes }}</td></tr>
    {% endfor %}
  </tbody>
</table-->      



<script type="text/javascript">
$(document).ready( function () {
    $('#table_id').DataTable();
} );
</script>