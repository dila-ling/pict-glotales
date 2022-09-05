---
layout: page
title: Corpus interno
permalink: /corpus-interno/
---

<div>
Esta sección sintetiza las características básicas del corpus usado para el proyecto. 

<!-- Agregar referencias bibliograficas y cuadritos de cantidad de palabras por fuente y por idioma -->

<h2>Documentos</h2>

<table id="table_00" class="display table py-2 mb-4">
  <thead>
    <tr>
        <th>Archivo</th>
        <th>Formato</th>
        <th>Código</th>
        <th>Cita</th>
        <th>Lengua</th>
        <th>Soporte</th>
        <th>Tipo</th>
    </tr>
  </thead>
  <tbody>
  {% for row in site.data.map_archivos_ref_biblio %}
    <tr>
        <td>{{ row.Archivo }}</td>
        <td>{{ row.Formato }}</td>
        <td>{{ row.Codigo }}</td>
        <td><button class="balloon" data-balloon-pos="up" data-balloon-length="large" data-balloon="{{row.Referencia}}">{{ row.Cita }}</button></td>
        <td>{{row.Lengua}}</td>
        <td>{{row.Soporte}}</td>
        <td>{{row.Tipo}}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>  


<h2>Corpus de audio</h2>

<p>Registros de audio de entrevistas de trabajo de campo.</p>

<table id="table_01" class="display table py-2 mb-4">
  <thead>
    <tr>
        <th>Archivo</th>
        <th>Lengua</th>
        <th>Palabras</th>
        <th>Duración (min)</th>
        <th>Líneas</th>
        <th>Comentario</th>
        <th>Transcriptorx</th>
        <th>Tanda</th>
        <th>Fuente</th>
        <th>Código</th>
    </tr>
  </thead>
  <tbody>
  {% for row in site.data.audiofiles_info %}
    <tr>
        <td>{{ row.Archivo }}</td>
        <td>{{ row.Lengua }}</td>
        <td>{{ row.Palabras }}</td>
        <td>{{ row.Dur }}</td>
        <td>{{row.Lineas}}</td>
        <td>{{row.Comentario}}</td>
        <td>{{row.Transcriptorx}}</td>
        <td>{{row.Tanda}}</td>
        <td>{{row.Fuente}}</td>
        <td>{{row.Codigo}}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>  

<h2>Textos</h2>

<p>Diccionarios, léxicos, tesis, etc.</p>

<table id="table_02" class="display table py-2 mb-4">
  <thead>
    <tr>
        <th>Archivo</th>
        <th>Lengua</th>
        <th>Código</th>
        <th>Tamaño(Mb)</th>
        <th>Páginas</th>
        <th>Líneas</th>
        <th>Palabras</th>
        <th>Cita</th>
    </tr>
  </thead>
  <tbody>
  {% for row in site.data.textfiles_info %}
    <tr>
        <td>{{ row.Archivo }}</td>
        <td>{{ row.Lengua }}</td>
        <td>{{ row.Codigo }}</td>
        <td>{{ row.Tamano }}</td>
        <td>{{ row.Paginas }}</td>
        <td>{{ row.Lineas }}</td>
        <td>{{ row.Palabras }}</td>
        <td><button class="balloon" data-balloon-pos="up" data-balloon-length="large" data-balloon="{{row.Referencia}}">{{ row.Cita }}</button></td>
    </tr>
  {% endfor %}
  </tbody>
</table>  

<div>

<script type="text/javascript">
$(document).ready( function () {
    $('#table_00').DataTable();
    $('#table_01').DataTable();
    $('#table_02').DataTable();
} );
</script>