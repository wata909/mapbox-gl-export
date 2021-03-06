# mapbox-gl-export
![](https://github.com/watergis/mapbox-gl-export/workflows/Node.js%20Package/badge.svg)
![GitHub](https://img.shields.io/github/license/watergis/mapbox-gl-export)

This module adds control which can export PDF and images.

This module is using source code of [mpetroff/print-maps](https://github.com/mpetroff/print-maps). I just adopted this library to normal Mapbox GL Plugin. Thanks so much to develop this library!

## Installation:

```bash
npm i @watergis/mapbox-gl-export --save
```

## Demo:

See [demo](https://watergis.github.io/mapbox-gl-export/#12/-1.08551/35.87063).

![demo.gif](./demo.gif)

## Test:

```
npm run build
npm start
```

open [http://localhost:8080](http://localhost:8080).

## Usage:

```ts
import MapboxExportControl from "@watergis/mapbox-gl-export";
import '@watergis/mapbox-gl-export/css/styles.css';
import mapboxgl from 'mapbox-gl';

const map = new mapboxgl.Map();
map.addControl(new MapboxExportControl(), 'top-right');
});
```

## Attribution

When you use exported map, please includes attribution as follows.

If you can include HTML, use this code snippet that includes links to Mapbox & OpenStreetMap:
```html
© NARWASSCO, Ltd. © <a href='https://www.mapbox.com/about/maps/'>Mapbox</a> © <a href='https://www.openstreetmap.org/copyright'>OpenStreetMap</a> <strong><a href='https://www.mapbox.com/map-feedback/' target='_blank'>Improve this map</a></strong>Powered by the United Nations Vector Tile Toolkit
```

For print output or if you can’t include links, use this text-only attribution:
```
© NARWASSCO, Ltd. ©Mapbox ©OpenStreetMap contributors, Powered by the United Nations Vector Tile Toolkit
```

`© NARWASSCO, Ltd.` is default example of map data by `Narok Water and Sewerage Services Co., Ltd.`, Kenya. If you don't use current map, you don't need to use this attribution.

Also, default example is using base map by United Nation Vector Tile Toolkit. That is why `Powered by the United Nations Vector Tile Toolkit` is included in above.

## Contribution

This Mapbox GL Export Control is still under development. so most welcome any feedbacks and pull request to this repository.
