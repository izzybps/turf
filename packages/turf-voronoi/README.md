# @turf/voronoi

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## voronoi

Takes a collection of points and a bounding box, and returns a collection
of Voronoi polygons.

The Voronoi algorithim used comes from the d3-voronoi package.

### Parameters

*   `points` **[FeatureCollection][1]<[Point][2]>** points around which to calculate the Voronoi polygons
*   `options` **[Object][3]** Optional parameters (optional, default `{}`)

    *   `options.bbox` **[BBox][4]** clipping rectangle, in \[minX, minY, maxX, MaxY] order (optional, default `[-180,-85,180,-85]`)

### Examples

```javascript
const options = {
  bbox: [-70, 40, -60, 60]
};
const points = turf.randomPoint(100, options);
const voronoiPolygons = turf.voronoi(points, options);

//addToMap
const addToMap = [voronoiPolygons, points];
```

Returns **[FeatureCollection][1]<[Polygon][5]>** a set of polygons, one per input point

[1]: https://tools.ietf.org/html/rfc7946#section-3.3

[2]: https://tools.ietf.org/html/rfc7946#section-3.1.2

[3]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[4]: https://tools.ietf.org/html/rfc7946#section-5

[5]: https://tools.ietf.org/html/rfc7946#section-3.1.6

<!-- This file is automatically generated. Please don't edit it directly. If you find an error, edit the source file of the module in question (likely index.js or index.ts), and re-run "yarn docs" from the root of the turf project. -->

---

This module is part of the [Turfjs project](https://turfjs.org/), an open source module collection dedicated to geographic algorithms. It is maintained in the [Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create PRs and issues.

### Installation

Install this single module individually:

```sh
$ npm install @turf/voronoi
```

Or install the all-encompassing @turf/turf module that includes all modules as functions:

```sh
$ npm install @turf/turf
```
