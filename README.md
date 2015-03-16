# turf-vincenty-inverse

[![Build Status](https://travis-ci.org/Turfjs/turf-vincenty-inverse.svg?branch=master)](https://travis-ci.org/Turfjs/turf-vincenty-inverse)

turf distance module


### `turf.vincenty-inverse(from, to, units)`

Vincenty's inverse formula computes the geographical distance and direction between two given points.

### Parameters

| parameter            | type               | description                                               |
| -------------------- | ------------------ | --------------------------------------------------------- |
| `from`               | Feature\.\<Point\> | origin point                                              |
| `to`                 | Feature\.\<Point\> | destination point                                         |
| `[units=kilometers]` | String             | _optional:_ can be degrees, radians, miles, or kilometers |


### Example

```js
var point1 = turf.point([-75.343, 39.984]);
var point2 = turf.point([-75.534, 39.123]);

var points = turf.featurecollection([point1, point2]);

//=points

var distance = turf.vincenty-inverse(point1, point2);

//=distance
```

## Installation

Requires [nodejs](http://nodejs.org/).

```sh
$ npm install turf-vincenty-inverse
```

## Tests

```sh
$ npm test
```