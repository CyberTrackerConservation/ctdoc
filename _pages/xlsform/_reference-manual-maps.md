## Offline maps

### What is an offline map?
Offline maps are map layers that are installed in CyberTracker. They can be used on the Map page. With the exception of WMS layers, they do not require a network connection.

### Packages
An offline map package is a zip file containing one or more layer files. See this [sample]({{ site.baseurl }}/assets/xlsform/offlinemap.zip) file. Note that the `layers.json` file is optional - by default the system will automatically discover files with supported extensions. Many map layers require several files with the same base name, for example shape files require a .shp, .shx, .dbf and .prj file. These should all be in the base directory of the zip file.

### Package installation
On **desktop**, a map package can be installed using `Install package` from the `File` menu.

On **mobile**, maps can also be installed directly from the `Offline maps` page. This can be reached via `Settings` or the gear icon on the Map Layers page:
<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-offlinemap-1.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-offlinemap-2.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-offlinemap-3.png" /></td>
</tr>
</table>

### Layer order and opacity
CyberTracker will discover and install layers in a zip file automatically. While this is often acceptable, when there are multiple layers, it is useful to specify the order and opacity of each. To do this, add a `layers.json` file to the zip and specify each of the layers:

```json
[
    {
        "filename": "Gabon.mbtiles",
        "name": "Gabon",
        "active": true,
        "opacity": 1.0
    },
    {
        "filename": "Country.shp",
        "name": "World countries",
        "active": true,
        "opacity": 0.5
    },
    {
        "filename": "LegalAtlasShapeFile.shp",
        "legalAtlas": true,
        "name": "Legal atlas shapefile",
        "active": true,
        "opacity": 0.1,
        "symbol": {
           "fill-style": "solid",
           "fill-color": "#808080",
           "outline-symbol": {
              "stroke-style": "dashdot",
              "stroke-size": 1.0,
              "stroke-color": "#404040"
           }  
    }
]
```

Note that the Settings page for offline maps also supports re-ordering the layers, sharing with others and even deleting them:
<table>
<tr>
<td><img width="240" src="{{ site.baseurl }}/assets/xlsform/refman-offlinemap-4.png" /></td>
</tr>
</table>

### Sharing
Offline map packages can be shared to other devices. This shares the entire original package, not just the selected layer. 

### Zoom to layer

On the Map Layers page, selecting the `Zoom to` button will zoom to the entire extent of the layer.

<table>
<tr>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-offlinemap-5.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-offlinemap-6.png" /></td>
<td><img src="{{ site.baseurl }}/assets/xlsform/refman-offlinemap-7.png" /></td>
</tr>
</table>

### Supported formats

The following layer formats are supported:
- ESRI formats: shapefile (shp), tile package (tpk), vector tiles package (vtpk)
- ASRP/USRP
- CIB1, 5, 10
- DTED0, 1, 2
- GeoTIFF
- HFA
- HRE
- IMG
- JPEG
- JPEG 2000
- NITF
- PNG
- RPF
- SRTM1, 2
- Mosaic Dataset in SQLite (read-only)
- MapBox: mbtiles 
- Google: KML
- GeoJSON

### Shape files
Shape files entries can include symbology.

#### Point symbols
`marker-style` can be `circle`, `cross`, `diamond`, `square`, `triangle`, `x`.
```json
"symbol": {
    "marker-style": "circle",
    "marker-size": 5.5,
    "marker-color": "#ffff00",
    "outline-color": "#ff0000"
}
```
#### Line symbols
`stroke-style` can be `solid`, `dash`, `dashdot`, `dashdotdot`, `dot`.
```json
"symbol": {
    "stroke-style": "dashdot",
    "stroke-size": 4.4,
    "stroke-color": "#ffff00"
}
```

#### Line symbols
`fill-style` can be `none`, `solid`, `horizontal`, `vertical`, `forwardDiagonal`, `backwardDiagonal`, `cross`, `diagonalCross`.
```json
"symbol": {
   "fill-style": "solid",
   "fill-color": "#ff00ff",
   "outline-symbol": {
      "stroke-style": "dashdot",
      "stroke-size": 1.0,
      "stroke-color": "#ffff00"
   }  
}
```

### WMS layers

[Web Map Service](https://wikipedia.org/wiki/Web_Map_Service) is an online layer protocol. While these layers are actually online, they can be added as layers using the Offline map system. To do this, create a JSON file with the extension `.wms` and add it to the package zip file. For example:

```json
{
    "layer": "0",
    "service": "https://basemap.nationalmap.gov/arcgis/services/USGSHydroCached/MapServer/WMSServer"
}
```
