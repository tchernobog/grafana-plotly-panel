## Plot.ly Panel for Grafana

[![CircleCI](https://circleci.com/gh/NatelEnergy/grafana-plotly-panel/tree/master.svg?style=svg)](https://circleci.com/gh/NatelEnergy/grafana-plotly-panel/tree/master)
[![dependencies Status](https://david-dm.org/NatelEnergy/grafana-plotly-panel/status.svg)](https://david-dm.org/NatelEnergy/grafana-plotly-panel)
[![devDependencies Status](https://david-dm.org/NatelEnergy/grafana-plotly-panel/dev-status.svg)](https://david-dm.org/NatelEnergy/grafana-plotly-panel?type=dev)

Render metrics using the plot.ly javascript framework

Works with grafana 4 and 5

### Screenshots

![Screenshot of scatter plot](https://raw.githubusercontent.com/NatelEnergy/grafana-plotly-panel/master/src/img/screenshot-scatter.png)
![Screenshot of scatter plot](https://github.com/CorpGlory/grafana-plotly-panel/blob/new-screenshots/src/img/screenshot-single-trace.png?raw=true)
![Screenshot of scatter plot](https://github.com/CorpGlory/grafana-plotly-panel/blob/new-screenshots/src/img/screenshot-multiple-trace.png?raw=true)
![Screenshot of 3d scatter plot](https://raw.githubusercontent.com/NatelEnergy/grafana-plotly-panel/master/src/img/screenshot-scatter-3d.png)
![Screenshot of the options screen](https://github.com/CorpGlory/grafana-plotly-panel/blob/new-screenshots/src/img/screenshot-options-new.png?raw=true)

### Building

To complie, run:

```
npm install -g yarn
yarn install --pure-lockfile
yarn build
```

#### Changelog

##### v0.0.5 (not released yet)

* Upgrade plotly (v1.39+)
* Better support for light theme. (#24, @cscheuermann81)
* Support snapshots
* Removing `dist` from master branch
* Support of multiple time series's ([#9](https://github.com/NatelEnergy/grafana-plotly-panel/issues/9), [CorpGlory DevTeam](https://corpglory.com/))
* Support showing text from query (#11)

##### v0.0.4

* Load plotly from npm (v1.31.2+)
* Convert to TypeScript
* Reasonable behavior when adding single metric
* Formatting with prettier.js
* Support for a single table query

##### v0.0.3

* Improve options UI
* Added range mode: "tozero" and "nonnegative"
* Map metrics to X,Y,Z and color
* Can now select 'date' type for each axis to support time
* basic support to size marker with data

##### v0.0.2

* Added ability to set color from a metric query. (#4, @lzgrablic01)
* Show 3D axis names properly
* Fix initalization to work with 4.2+ (isPanelVisible undefined)

##### v0.0.1

* First working version

### Roadmap

* support 'table' response format for more than one query.

Nice things to have

* sizeref helper. I think this depends on the data. likely need to find the range and pick a good value?
* support text
* load plotly.js from CDN?
* nice to have: https://plot.ly/javascript/parallel-coordinates-plot/
