---
layout: page
title: Resultados
permalink: /resultados/
---


# Mataguayas comparadas

<div class="py-1 mb-0 ml-3 prose">
  <a class="no-underline" data-toggle="collapse" href="#texto" role="button" aria-expanded="false" aria-controls="collapseExample">
    <h3>Comparación de fuentes textuales <span class="caret"/></h3></a>
  <div class="collapse py-2" id="texto">
    <p>Cuadro con vocabulario comparado de lenguas mataguayas. Las transcripciones originales registradas en la bibliografía fueron adaptadas al Alfabeto Fonético Internacional. No se modificaron las vocales dobles ya que pueden implicar distintos símbolos fonéticos.</p>
    <p>Deslice el cursor sobre las palabras para ver la fuente textual.</p>
    <table id="table_01" class="display table py-2 mb-4">
      <thead>  
        <tr>
          <th>Español</th>
          <th>Wichi</th>
          <th>Chorote</th>
          <th>Nivaĉle</th>
          <th>Maka</th>
        </tr>
      </thead>
      <tbody>
      {% for row in site.data.mataguayas-comparadas-AG %}
      <tr>
        <td>{{ row.espanol }}</td>
        <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_wichi}}">{{ row.wichi }}</button></td>
        <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_chorote}}">{{ row.chorote }}</button></td>
        <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_nivacle}}">{{ row.nivacle }}</button></td>
        <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_maka}}">{{ row.maka }}</button></td>
      </tr> 
      {% endfor %}
    </tbody>
    </table>
  </div>

  <a class="no-underline" data-toggle="collapse" href="#audio" role="button" aria-expanded="false" aria-controls="collapseExample"><h3>Comparación de fuentes de audio <span class="caret"/></h3></a>
  <div class="collapse py-2" id="audio">
    <p>Cuadro con vocabulario comparado de lenguas mataguayas proveniente de <a href="{{site.baseurl}}/transcripciones/">transcripciones</a> de 9h de elicitaciones de trabajo de campo.</p>
    <p>Deslice el cursor sobre las palabras para ver la fuente textual.</p>
    <table id="table_02" class="display table py-2 mb-4">
      <thead>
        <tr>
          <th>Español</th>
          <th>Wichi</th>
          <th>Chorote</th>
          <th>Nivaĉle</th>
          <th>Maka</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.mataguayas-comparadas-audio %}
          <tr>
            <td>{{ row.espanol }}</td>
            <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_wichi}}">{{ row.wichi }}</button></td>
            <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_chorote}}">{{ row.chorote }}</button></td>
            <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_nivacle}}">{{ row.nivacle }}</button></td>
            <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_maka}}">{{ row.maka }}</button></td>
          </tr> 
        {% endfor %}
      </tbody>
    </table>
  </div>
</div>

<script type="text/javascript">
$(document).ready( function () {
    $('#table_01').DataTable();
    $('#table_02').DataTable();
} );
</script>