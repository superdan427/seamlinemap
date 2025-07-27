<!DOCTYPE html>
<html>
  <head>
    <title>Seamline Map</title>
    <style>
      html, body, #map {
        height: 100%;
        margin: 0;
        padding: 0;
      }
    </style>
    <script src="https://maps.googleapis.com/maps/api/js?key=AIzaSyD9CHMD2CaGELMCa2gDIptRdhBzw89N_JA"></script>
    <script>
      const mapStyle = [
        {
          "elementType": "geometry",
          "stylers": [{ "color": "#f5f5f5" }]
        },
        {
          "elementType": "labels.icon",
          "stylers": [{ "visibility": "off" }]
        },
        {
          "elementType": "labels.text.fill",
          "stylers": [{ "color": "#616161" }]
        },
        {
          "elementType": "labels.text.stroke",
          "stylers": [{ "color": "#f5f5f5" }]
        },
        {
          "featureType": "administrative.land_parcel",
          "elementType": "labels.text.fill",
          "stylers": [{ "color": "#bdbdbd" }]
        },
        {
          "featureType": "administrative.neighborhood",
          "stylers": [{ "visibility": "off" }]
        },
        {
          "featureType": "poi",
          "elementType": "geometry",
          "stylers": [{ "color": "#eeeeee" }]
        },
        {
          "featureType": "poi",
          "elementType": "labels.text",
          "stylers": [{ "visibility": "off" }]
        },
        {
          "featureType": "poi",
          "elementType": "labels.text.fill",
          "stylers": [{ "color": "#757575" }]
        },
        {
          "featureType": "poi.business",
          "stylers": [{ "visibility": "off" }]
        },
        {
          "featureType": "poi.park",
          "elementType": "geometry",
          "stylers": [{ "color": "#e5e5e5" }]
        },
        {
          "featureType": "poi.park",
          "elementType": "labels.text",
          "stylers": [{ "visibility": "off" }]
        },
        {
          "featureType": "poi.park",
          "elementType": "labels.text.fill",
          "stylers": [{ "color": "#9e9e9e" }]
        },
        {
          "featureType": "road",
          "elementType": "geometry",
          "stylers": [{ "color": "#ffffff" }]
        },
        {
          "featureType": "road",
          "elementType": "labels",
          "stylers": [{ "visibility": "off" }]
        },
        {
          "featureType": "road.arterial",
          "elementType": "labels.text.fill",
          "stylers": [{ "color": "#757575" }]
        },
        {
          "featureType": "road.highway",
          "elementType": "geometry",
          "stylers": [{ "color": "#dadada" }]
        },
        {
          "featureType": "road.highway",
          "elementType": "labels.text.fill",
          "stylers": [{ "color": "#616161" }]
        },
        {
          "featureType": "road.local",
          "elementType": "labels.text.fill",
          "stylers": [{ "color": "#9e9e9e" }]
        },
        {
          "featureType": "transit.line",
          "elementType": "geometry",
          "stylers": [{ "color": "#e5e5e5" }]
        },
        {
          "featureType": "transit.station",
          "elementType": "geometry",
          "stylers": [{ "color": "#eeeeee" }]
        },
        {
          "featureType": "water",
          "elementType": "geometry",
          "stylers": [{ "color": "#c9c9c9" }]
        },
        {
          "featureType": "water",
          "elementType": "labels.text",
          "stylers": [{ "visibility": "off" }]
        },
        {
          "featureType": "water",
          "elementType": "labels.text.fill",
          "stylers": [{ "color": "#9e9e9e" }]
        }
      ];

      function initMap() {
        new google.maps.Map(document.getElementById("map"), {
          center: { lat: 51.5074, lng: -0.1278 }, // London
          zoom: 12,
          styles: mapStyle
        });
      }
    </script>
  </head>
  <body onload="initMap()">
    <div id="map"></div>
  </body>
</html>
