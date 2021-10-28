# Implementacion de Mapas usando OpenLayers
Deben tener instalado yarn o npm para hacer la corrida. Luego solo necesitan correr el script "parcel_install.ps1" (powershell/windows) o el "parcel_install.sh" (bash/linux). El script instalara parcel utilizando yarn o npm y lo montara en http://localhost:1234. Para modificar la ubicación deben cambiar la informacion del lugar en el archivo "main.js"


```javascript
//Para hacer cambios en la ubicación solo hay que cambiar la ubicación.
const place = [-69.93855751772563,18.481367130149952];
```

Tambien esta la versión simplificada en el archivo "index_simplified.html". La cual la pueden correr directamente como pagina estatica. Solo seria cambiar el segmento donde se envian las coordenadas.

```javascript
var map = new ol.Map({
target: 'map',
layers: [
    new ol.layer.Tile({
    source: new ol.source.OSM()
    })
],
view: new ol.View({
    center: ol.proj.fromLonLat([-69.93855751772563,18.481367130149952]),
    zoom: 18
})
});
```


##Uso 
Para ponerlo a correr luego solo hay que correr. 
Cuando se utiliza yarn:
```bash
yarn start
```


## Mas Infomración
[OpenLayers](https://openlayers.org/)