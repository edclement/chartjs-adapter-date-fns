# chartjs-adapter-date-fns

[![release](https://img.shields.io/github/release/chartjs/chartjs-adapter-date-fns.svg?style=flat-square)](https://github.com/chartjs/chartjs-adapter-date-fns/releases/latest) [![travis](https://img.shields.io/travis/chartjs/chartjs-adapter-date-fns.svg?style=flat-square&maxAge=60)](https://travis-ci.org/chartjs/chartjs-adapter-date-fns) [![awesome](https://awesome.re/badge-flat2.svg)](https://github.com/chartjs/awesome)

## Overview

This adapter allows to use date-fns with the Chart.js.

Requires [Chart.js](https://github.com/chartjs/Chart.js/releases) **2.8.0** or later and [date-fns](https://date-fns.org/) **1.30.1** or later.

## Getting started

### npm

```
npm install chartjs-adapter-date-fns --save
```

### CDN

By default, `https://cdn.jsdelivr.net/npm/chartjs-adapter-date-fns` returns the latest (minified) version, however it's [highly recommended](https://www.jsdelivr.com/features) to always specify a version in order to avoid breaking changes. This can be achieved by appending `@{version}` to the url:

```
https://cdn.jsdelivr.net/npm/chartjs-adapter-date-fns@0.1.0
```

Read more about jsDeliver versioning on their [website](http://www.jsdelivr.com/).

## Integration

**Note:** once loaded, this adapter overrides the default date-adapter provided in Chart.js (as a side-effect).

### HTML

```html
<script src="https://cdn.jsdelivr.net/npm/chart.js@2.8.0/dist/Chart.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/date-fns@1.30.1/index.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chartjs-adapter-date-fns@0.1.0"></script>
```

### Module

```javascript
import Chart from 'chart.js';
import 'chartjs-adapter-date-fns';
```

## Configuration

No adapter configuration is currently available, read the [Chart.js documention](https://www.chartjs.org/docs/latest) for other possible date/time related options. For example, the time scale [`time.*` options](https://www.chartjs.org/docs/latest/axes/cartesian/time.html#configuration-options) can be overridden using the [date-fns tokens](https://date-fns.org/v1.30.1/docs/format).

## Development

You first need to install node dependencies (requires [Node.js](https://nodejs.org/)):

```
> npm install
```

The following commands will then be available from the repository root:

```
> gulp build            // build dist files
> gulp build --watch    // build and watch for changes
> gulp lint             // perform code linting
```

## License

`chartjs-adapter-date-fns` is available under the [MIT license](LICENSE.md).
