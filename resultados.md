---
layout: page
title: Resultados
permalink: /resultados/
---


# Mataguayas comparadas

<div class="py-1 mb-0 prose">
  <h3>Comparación de fuentes textuales</h3>
  <div class="py-2" id="texto">
    <p>Vocabulario comparado de lenguas mataguayas. Las transcripciones originales registradas en la bibliografía fueron adaptadas al Alfabeto Fonético Internacional. No se modificaron las vocales dobles ya que pueden implicar distintos símbolos fonéticos.</p>
    <p>Deslice el cursor sobre las palabras para ver la fuente textual. La lista de referencias bibliográficas completas puede consultarse debajo de la tabla.</p>
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
    <a class="no-underline" data-toggle="collapse" href="#bib1" role="button" aria-expanded="false" aria-controls="collapseExample"><h4>Ver referencias <span class="caret"/></h4></a>
    <div class="collapse py-2" id="bib1">
      {% assign handle = "text" %}
      {% include referencias_biblio.html %}
    </div>
  </div>

 <h3>Comparación de fuentes de audio</h3>
  <div class="py-2" id="audio">
    <p>Vocabulario comparado de lenguas mataguayas proveniente de <a href="{{site.baseurl}}/transcripciones/">transcripciones</a> de 9h de elicitaciones de trabajo de campo.</p>
    <p>Deslice el cursor sobre las palabras para ver la fuente y haga click sobre 🔉 para reproducir el audio. La lista de fuentes de registros de audio puede consultarse debajo de la tabla.</p>
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
            <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_wichi}}">{{ row.wichi }}</button>{% if row.audio_wichi != nil %} <span class="pointer" onclick="playAudio('{{ site.baseurl }}/assets/audio/{{row.audio_wichi}}.wav')" type="button">🔉</span>{% endif %}</td>
            <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_chorote}}">{{ row.chorote }}</button>{% if row.audio_chorote != nil %} <span class="pointer" onclick="playAudio('{{ site.baseurl }}/assets/audio/{{row.audio_chorote}}.wav')" type="button">🔉</span>{% endif %}</td>
            <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_nivacle}}">{{ row.nivacle }}</button>{% if row.audio_nivacle != nil %} <span class="pointer" onclick="playAudio('{{ site.baseurl }}/assets/audio/{{row.audio_nivacle}}.wav')" type="button">🔉</span>{% endif %}</td>
            <td><button class="balloon" data-balloon-pos="up" data-balloon-length="small" data-balloon="{{row.fuente_maka}}">{{ row.maka }}</button>{% if row.audio_maka != nil %} <span class="pointer" onclick="playAudio('{{ site.baseurl }}/assets/audio/{{row.audio_maka}}.wav')" type="button">🔉</span>{% endif %}</td>
          </tr> 
        {% endfor %}
      </tbody>
    </table>
    <a class="no-underline" data-toggle="collapse" href="#bib2" role="button" aria-expanded="false" aria-controls="collapseExample"><h4>Ver referencias <span class="caret"/></h4></a>
    <div class="collapse py-2" id="bib2">
      {% assign handle = "audio" %}
      {% include referencias_biblio.html %}
    </div>
  </div>
</div>

<script type="text/javascript">
$(document).ready( function () {
    $('#table_01').DataTable();
    $('#table_02').DataTable();
} );
</script>

<script type="text/javascript">
function playAudio(url) { 
  new Audio(url).play(); 
}
</script>