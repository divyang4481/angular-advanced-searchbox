## Angular Advanced Searchbox
[![Build Status](https://travis-ci.org/dnauck/angular-advanced-searchbox.png?branch=master)](https://travis-ci.org/dnauck/angular-advanced-searchbox)

A directive for AngularJS providing a advanced visual search box.

### [DEMO](http://dnauck.github.io/angular-advanced-searchbox/)

### Usage

Include with bower

```sh
bower install angular-advanced-searchbox
```

Load the javascript and css and declare your Angular dependency

```html
<link rel="stylesheet" href="angular-advanced-searchbox.min.css">
<script src="angular-advanced-searchbox.min.js"></script>
```

```js
angular.module('myModule', ['angular-advanced-searchbox']);
```

Then in your view

```html
<nit-advanced-searchbox
	ng-model="searchParams"
	parameters="availableSearchParams"
	placeholder="Search...">
</nit-advanced-searchbox>
```

The `angular-advanced-searchbox` directive uses an external template stored in
`angular-advanced-searchbox.html`.  Host it in a place accessible to
your page and set the `template-url` attribute. Note that the `url`
param can be a scope variable as well as a hard-coded string.

### Benefits

* Handles free text search and/or parameterized searches
* Provides suggestions on available search parameters
* Easy to use with mouse or keyboard
* Model could easily be used as ```params``` for Angular's ```$http``` API
* Twitter Bootstrap compatible markup
* Works perfectly together with [angular-paginate-anything](https://github.com/begriffs/angular-paginate-anything) (use ```ng-model``` as ```url-params```)

### Directive Attributes

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ng-model</td>
      <td>Search parameters as object that could be used as <i>params</i> with Angular's <i>$http</i> API.</td>
    </tr>
    <tr>
      <td>parameters</td>
      <td>List of available parameters to search for.</td>
    </tr>
    <tr>
      <td>placeholder</td>
      <td>specifies a short hint in the search box</td>
    </tr>
  </tbody>
</table>
