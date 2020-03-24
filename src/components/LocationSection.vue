<template>
  <section id="location-section">
    <div class="wrapper">

      <div id="map" ref="map"></div>

    </div>
  </section>
</template>

<script>
import postscribe from 'postscribe'

export default {
  name: 'CommunitySection',
  data: function() {
    return {
      map: null
    }
  },
  methods: {
    initMap: function() {
        this.map = new google.maps.Map(this.$refs["map"], {
          center: {lat: 51.5124319, lng: -0.1290983},
          zoom: 14,
          zoomControl: true,
          mapTypeControl: false,
          scaleControl: false,
          streetViewControl: false,
          rotateControl: false,
          fullscreenControl: false,
          styles: [{
        		"featureType": "landscape",
        		"stylers": [
                  			{
                  				"hue": "#FF5300"
                  			},
                  			{
                  				"saturation": 100
                  			},
                  			{
                  				"lightness": 22.82352941176468
                  			},
                  			{
                  				"gamma": 1
                  			}
                  		]
          	},
          	{
          		"featureType": "road.highway",
          		"stylers": [
          			{
          				"hue": "#FF0300"
          			},
          			{
          				"saturation": -100
          			},
          			{
          				"lightness": 61.39999999999998
          			},
          			{
          				"gamma": 1
          			}
          		]
          	},
          	{
          		"featureType": "road.arterial",
          		"stylers": [
          			{
          				"hue": "#FF0300"
          			},
          			{
          				"saturation": -100
          			},
          			{
          				"lightness": 51.19999999999999
          			},
          			{
          				"gamma": 1
          			}
          		]
          	},
          	{
          		"featureType": "road.local",
          		"stylers": [
          			{
          				"hue": "#FF0300"
          			},
          			{
          				"saturation": -100
          			},
          			{
          				"lightness": 52
          			},
          			{
          				"gamma": 1
          			}
          		]
          	},
          	{
          		"featureType": "water",
          		"stylers": [
          			{
          				"hue": "#00FFF3"
          			},
          			{
          				"saturation": 13.669064748201421
          			},
          			{
          				"lightness": -2.509803921568647
          			},
          			{
          				"gamma": 1
          			}
          		]
          	},
          	{
          		"featureType": "poi",
          		"stylers": [
                {
                  visibility: 'off'
                },
          		]
          	}
          ]
        });

        var image = 'https://raw.githubusercontent.com/thomascruz/studiographenetestexercise/master/src/assets/location-icon.svg?token=AAYGNRJNHLKD46M4W3DIEFS6QOMES';
        var beachMarker = new google.maps.Marker({
          position: {lat: 51.5124319, lng: -0.1290983},
          map: this.map,
          icon: image
        });
      }
  },
  mounted: function () {
    let self = this;

    postscribe('#location-section', "<script src='https://maps.googleapis.com/maps/api/js?key=AIzaSyCDrI0jygq2VAMUg8pVA35jps_8Ziu8PPs' defer><\/script>", {
      done: function() {
        self.initMap();
      }
    });

  }
}
</script>
