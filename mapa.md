---
layout: page
title: Mapa de fuentes
permalink: /mapa/
---


# Geolocalización de trabajo de campo

En este mapa se puede visualizar dónde fueron tomadas las muestras. Haga click sobre los marcadores para obtener más información. 

<br>


<div id="map" class="map leaflet-container" style="height: 500px; position:relative;"></div>

<script>
// create the map object and set the cooridnates of the initial view:
var map = L.map('map').setView([-24.5811123, -60.4287612], 6);

  L.tileLayer('https://api.mapbox.com/styles/v1/{id}/tiles/{z}/{x}/{y}?access_token={accessToken}', {
      attribution: 'Map data &copy; <a href="http://openstreetmap.org">OpenStreetMap</a>, <a href="http://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, Imagery © <a href="http://mapbox.com">Mapbox</a>',
      maxZoom: 18,
      tileSize: 512,
      zoomOffset: -1,
      id: 'mapbox/streets-v11',
      accessToken: 'pk.eyJ1IjoiaGRjYWljeXQiLCJhIjoiY2s5MDc0NGQ3MjBudTNtbWh1NzFmM2VjZyJ9.MuGwJ2d1CmhzIg4M-TQJWA'
  }).addTo(map);

  var marker = L.marker([-21.26, -63.45807]).addTo(map);
  marker.bindPopup("<h6>Villamontes</h6><br><b>Wichí</b>: Claesson, 2016");
  var marker = L.marker([-23.8988, -61.8546]).addTo(map);
  marker.bindPopup("<h6>Ing. Juárez</h6><br><b>Wichí</b>: Nercesian, 2014");
  var marker = L.marker([-24.2539, -61.2423]).addTo(map);
  marker.bindPopup("<h6>Laguna Yema</h6><br><b>Wichí</b>: Nercesian, 2014");
  var marker = L.marker([-24.4031, -61.0321]).addTo(map);
  marker.bindPopup("<h6>Pozo del Mortero</h6><br><b>Wichí</b>: Nercesian, 2014");
  var marker = L.marker([-24.5422, -60.8312]).addTo(map);
  marker.bindPopup("<h6>J.G.Bazán</h6><br><b>Wichí</b>: Nercesian, 2014");
  var marker = L.marker([-24.7075, -60.5943]).addTo(map);
  marker.bindPopup("<h6>Las Lomitas</h6><br><b>Wichí</b>: Nercesian, 2014");
  var marker = L.marker([-24.8958, -60.3194]).addTo(map);
  marker.bindPopup("<h6>Pozo del Tigre </h6><br><b>Wichí</b>: Nercesian, 2014");
  var marker = L.marker([-24.4236, -61.6842]).addTo(map);
  marker.bindPopup("<h6>Sauzalito </h6><br><b>Wichí</b>: Nercesian, 2014");
  var marker = L.marker([-24.92974, -61.48659]).addTo(map);
  marker.bindPopup("<h6>Nueva Pompeya</h6><br><b>Wichí</b>: Nercesian, 2014");
  var marker = L.marker([-22.368464519011034, -62.56198333139355]).addTo(map);
  marker.bindPopup("<h6>Misión La Paz</h6><br><b>Chorote</b>: Bucca, 1969; Carol, 2014a, 2014b; Drayson, 2009; Gerzenstein, 1978, 1979, 1983; Najlis, 1984;<br><b>Nivaclé</b>: Bucca, 1966, 1969; Campbell y Grondona, 2007; Najlis, 1984<br><b>Wichí</b>: Bucca, 1969");
  var marker = L.marker([-22.359316652886253, -60.03410410746284]).addTo(map);
  marker.bindPopup("<h6>Filadelfia</h6><br><b>Nivaclé</b>: Fabre, 2014");
  var marker = L.marker([-22.362071530572994, -60.050069732203234]).addTo(map);
  marker.bindPopup("<h6>Uj’e Lhavos</h6><br><b>Nivaclé</b>: Gutiérrez, 2015; Seelwische, 2016");
  var marker = L.marker([-22.040250843402525, -60.584650935243566]).addTo(map);
  marker.bindPopup("<h6>Misión Santa Teresita</h6><br><b>Nivaclé</b>: Gutiérrez, 2015; Seelwische, 2016");
  var marker = L.marker([-22.448409166690375, -62.34991587416593]).addTo(map);
  marker.bindPopup("<h6>Doctor Pedro P. Peña</h6><br><b>Nivaclé</b>: Seelwische, 2016");
  var marker = L.marker([-23.778712480052523, -60.78093582869899]).addTo(map);
  marker.bindPopup("<h6>Misión San Leonardo</h6><br><b>Nivaclé</b>: Seelwische, 2016");
  var marker = L.marker([-25.202873703397945, -57.525282620648575]).addTo(map);
  marker.bindPopup("<h6>Roque Mariano Alonso</h6><br><b>Maká</b>: Gerzenstein, 1985, 1994, 1999; Tacconi, 2015");
  var marker = L.marker([-24.0901755, -62.3430565]).addTo(map);
  marker.bindPopup("<h6>Misión Yacaré</h6><br><b>Chorote</b>: Najlis, 1984");
  var marker = L.marker([-23.26014811675107, -63.74069536741488]).addTo(map);
  marker.bindPopup("<h6>Mision Chaqueña</h6><br><b>Chorote</b>: Najlis, 1984");
  var marker = L.marker([-22.1918, -63.6371]).addTo(map);
  marker.bindPopup("<h6>El algarrobal</h6><br><b>Chorote</b>: Najlis, 1984");
  var marker = L.marker([-24.082252103507336, -62.3163828983847]).addTo(map);
  marker.bindPopup("<h6>Misión Pozo Yacaré</h6><br><b>Wichí</b>: Najlis, 1984");
  var marker = L.marker([-24.082252103507336, -62.3163828983847]).addTo(map);
  marker.bindPopup("<h6>Misión Algarrobal</h6><br><b>Wichí</b>: Najlis, 1984");
  var marker = L.marker([-23.778712480052523, -60.78093582869899]).addTo(map);
  marker.bindPopup("<h6>Misión San Leonardo, Asunción</h6><br>Chorote, Nivaclé, <b>Wichí</b>: Najlis, 1984");
  var marker = L.marker([-22.51856788662934, -63.79682502113404]).addTo(map);
  marker.bindPopup("<h6>Misión Chorote I, Parcela 42</h6><br><b>Chorote</b>: Carol, 2014a, 2014b; Pacor, 2005");
  var marker = L.marker([-22.526561359929403, -63.77337131789523]).addTo(map);
  marker.bindPopup("<h6>Lapacho I</h6><br><b>Chorote</b>: Carol, 2014a, 2014b");
  var marker = L.marker([-22.23295422489952, -62.68042784447631]).addTo(map);
  marker.bindPopup("<h6>La Merced</h6><br><b>Chorote</b>: Carol, 2014a, 2014b; Drayson, 2009; Pacor, 2005");
  var marker = L.marker([-23.82019487920117, -64.06324231944264]).addTo(map);
  marker.bindPopup("<h6>La Estrella</h6><br><b>Chorote</b>: Carol, 2014a, 2014b");
  var marker = L.marker([-22.37608027969886, -62.52214776834048]).addTo(map);
  marker.bindPopup("<h6>La gracia</h6><br><b>Chorote</b>: Drayson, 2009");
  var marker = L.marker([-23.2968, -62.1442]).addTo(map);
  marker.bindPopup("<h6>La Bolsa</h6><br><b>Chorote</b>: Drayson, 2009");
  var marker = L.marker([-22.51856788662934, -63.79682502113404]).addTo(map);
  marker.bindPopup("<h6>Tartagal</h6><br><b>Chorote</b>: Drayson, 2009");
  var marker = L.marker([-24.0901755, -62.3430565]).addTo(map);
  marker.bindPopup("<h6>Misión Yacaré</h6><br><b>Chorote</b>: Gerzenstein, 1978, 1979) ");
  var marker = L.marker([-23.26014811675107, -63.74069536741488]).addTo(map);
  marker.bindPopup("<h6>Mision Chaqueña</h6><br><b>Chorote</b>: Gerzenstein, 1978, 1979) ");
  var marker = L.marker([-22.1918, -63.6371]).addTo(map);
  marker.bindPopup("<h6>El algarrobal</h6><br><b>Chorote</b>: Gerzenstein, 1978, 1979) ");
  var marker = L.marker([-22.51856788662934, -63.79682502113404]).addTo(map);
  marker.bindPopup("<h6>Tartagal</h6><br><b>Chorote</b>: Gerzenstein, 1983");
  var marker = L.marker([-22.31133694343285, -60.23006034566219]).addTo(map);
  marker.bindPopup("<h6>Colonia 22</h6><br><b>Chorote</b>: Gerzenstein, 1983");
  var marker = L.marker([-21.692655524906407, -61.70568071149984]).addTo(map);
  marker.bindPopup("<h6>Santa rosa</h6><br><b>Chorote</b>: Gerzenstein, 1983");
  var marker = L.marker([-23.001267361979455, -56.099685619864026]).addTo(map);
  marker.bindPopup("<h6>Misión Nuevas tribus</h6><br><b>Chorote</b>: Gerzenstein, 1983");
  var marker = L.marker([-21.26, -63.45807]).addTo(map);
  marker.bindPopup("<h6>Villamontes</h6><br><b>Wichí</b>: Claesson, 1994");
  var marker = L.marker([-23.26014811675107, -63.74069536741488]).addTo(map);
  marker.bindPopup("<h6>Misión chaqueña, El algarrobal</h6><br><b>Chorote</b>: Gerzenstein,1968");
</script>