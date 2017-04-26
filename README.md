# React Leaflet Ant Path

## *A port of Leaflet AntPath for React Leaflet* 
[Demo of the Leaflet AntPath](http://rubenspgcavalcante.github.io/leaflet-ant-path)  
[Original plugin](https://github.com/rubenspgcavalcante/leaflet-ant-path/)  
[React Leaflet](https://github.com/PaulLeCam/react-leaflet)

## Contributing
Want to help? Open a [issue](https://github.com/rubenspgcavalcante/react-leaflet-ant-path/issues) or make a PR!  
Also, see the guide on [how to contribute](/.github/contributing.md).

### Installing
Via NPM:
```
 npm install leaflet-ant-path
```

### Requirements
  - leaflet >= v1
  - react >= v15
  - react-leaflet >= v1
  - leaflet-ant-path > v0.6.2
    

### Using the plugin
The AntPath component is exported by default:  

```jsx
    import AntPath from "react-leaflet-ant-path";

    // ...
    <AntPath positions={latLngs} options={antPathOptions} />    
```

### Parameters
The same as the original plugin.

| name | type | example | description |
|------|------|---------| ------------|
|positions| L.LatLng[] **or** Array\[number, number\]  | \[ \[0, 10\], \[-20, 0\], ... \] | A array of latitude and longitudes (same as used in [Polyline constructor](http://leafletjs.com/reference.html#polyline) )
|options| Object  | {color: 'red', weight: 5, ...}  | Same as the [Polyline options](http://leafletjs.com/reference.html#polyline-options) plus the **extra** options bellow
|options.paused| boolean | true/false | Starts with the animation paused (default: false)
|options.pulseColor| string | #FF00FF | Adds a color to the dashed flux (default: 'white')
|options.delay | string | 120 | Add a delay to the animation flux (default: 400)
|options.dashArray| [number, number] **or** string | [15, 30] |The size of the animated dashes (default: "10, 20"). See also [the pattern](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/stroke-dasharray)

---

### License
This project is under the [MIT LICENSE](http://opensource.org/licenses/MIT)