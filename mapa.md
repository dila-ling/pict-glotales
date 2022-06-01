---
layout: page
title: Mapa lexical
permalink: /mapa/
---

# Esto es una prueba de visualización

En este mapa se puede visualizar dónde fueron tomadas las muestras. Haga click sobre los marcadores para obtener más información. 

<br>


<div id="map" class="map leaflet-container" style="height: 500px; position:relative;"></div>

<script>
// create the map object and set the cooridnates of the initial view:
var map = L.map('map').setView([-30.5811123, -58.4287612], 5);

  L.tileLayer('https://api.mapbox.com/styles/v1/{id}/tiles/{z}/{x}/{y}?access_token={accessToken}', {
      attribution: 'Map data &copy; <a href="http://openstreetmap.org">OpenStreetMap</a>, <a href="http://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, Imagery © <a href="http://mapbox.com">Mapbox</a>',
      maxZoom: 18,
      tileSize: 512,
      zoomOffset: -1,
      id: 'mapbox/streets-v11',
      accessToken: 'pk.eyJ1IjoiaGRjYWljeXQiLCJhIjoiY2s5MDc0NGQ3MjBudTNtbWh1NzFmM2VjZyJ9.MuGwJ2d1CmhzIg4M-TQJWA'
  }).addTo(map);

var marker = L.marker([-30.99, -51.49]).addTo(map);
marker.bindPopup("<b>jlaʼ</b><br>Campaña 2009.");

var marker = L.marker([-25.28, -57.66]).addTo(map);
marker.bindPopup("<b>inɬaʔa</b><br>Campaña 2011.");

var marker = L.marker([-25.22, -57.56]).addTo(map);
marker.bindPopup("<b>inʼxlapa</b><br>Campaña 2011.");

var marker = L.marker([-34.07, -55.69]).addTo(map);
marker.bindPopup("<b>in’xa?a</b><br>Campaña 2010.");

var marker = L.marker([-27.79, -64.27]).addTo(map);
marker.bindPopup("<b>ʼxlokje</b><br>Campaña 2011.");

var marker = L.marker([-22.80, -43.16]).addTo(map);
marker.bindPopup("<b>ɬaʔa</b><br>Campaña 2017.");

</script>