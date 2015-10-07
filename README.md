# geoxml3
[see example](http://www.geocodezip.com/geoxml3_test/v3_geoxml3_kmltest_linkto.html?lat=41.897573&lng=-87.749474&zoom=10&type=m&filename=cta.xml)
# Support
kmz\kml support (master branch)
Parser can handle not even links but bufferarrays (taken from http response or from ```<input> ``` for example)
## Other stuffs:
#### parserOptions extended with those callbacks:
```js
onAfterCreateGroundOverlay = function (overlay){}
```

```js
onAfterCreatePolyLine = function (polyLineGoogleMVCObject,placemark){}
```

```js
onAfterCreatePolygon = function (polygonGoogleMVCObject,placemark){}
```
##### you can create infowindow in your code and pass it to parserOptions
```js
parserOptions.infowindow = new Infowindow();
```