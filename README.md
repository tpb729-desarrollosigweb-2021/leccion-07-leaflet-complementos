# Leaflet - complementos
[Leaflet](https://leafletjs.com/) es una biblioteca diseñada para ser "liviana". Su funcionalidad básica puede ser extendida a través de [complementos o *plugins*](https://leafletjs.com/plugins.html), desarrollados por la comunidad de programadores de Leaflet.

## leaflet-providers
El complemento [leaflet-providers](https://github.com/leaflet-extras/leaflet-providers) simplifica el despliegue de capas de teselas de varios [proveedores](http://leaflet-extras.github.io/leaflet-providers/preview/).

Para utilizarse, primero debe descargarse el archivo [leaflet-providers.js](https://raw.githubusercontent.com/leaflet-extras/leaflet-providers/master/leaflet-providers.js) e incluir un enlace a este en el código JavaScript, después del enlace a Leaflet. 

```html
<head>
  ...
  <script src="http://unpkg.com/leaflet@1.3.1/dist/leaflet.js"></script>
  <script src="js/leaflet-providers.js"></script>
</head>
```

Luego, debe llamarse al constructor ```L.tileLayer.provider``` y pasarle como argumento la hilera que identifica al proveedor, como se muestra en [http://leaflet-extras.github.io/leaflet-providers/preview/](http://leaflet-extras.github.io/leaflet-providers/preview/).

```javascript
// Agregar mapa de Stamen Watercolor
L.tileLayer.provider('Stamen.Watercolor').addTo(map);
```

**Ejercicios**  
1. Tomando como base el código fuente disponible en [https://github.com/tpb729-desarrollosigweb-2021/ejemplo-mapa-leaflet-complementos](https://github.com/tpb729-desarrollosigweb-2021/ejemplo-mapa-leaflet-complementos) (y que puede visualizarse en [https://tpb729-desarrollosigweb-2021.github.io/ejemplo-mapa-leaflet-complementos/](https://tpb729-desarrollosigweb-2021.github.io/ejemplo-mapa-leaflet-complementos/)):
  a. agregue dos capas base adicionales utilizando el complemento leaflet-providers.
