# emberx-select-blockless

[![npm version](https://badge.fury.io/js/emberx-select-blockless.svg)](http://badge.fury.io/js/emberx-select-blockless)
[![Ember Observer Score](http://emberobserver.com/badges/emberx-select-blockless.svg)](http://emberobserver.com/addons/emberx-select-blockless)
[![Build Status](https://travis-ci.org/thefrontside/emberx-select-blockless.svg?branch=master)](https://travis-ci.org/thefrontside/emberx-select-blockless)


This Addon extends
[emberx-select](https://github.com/thefrontside/emberx-select) so that
it can be used in blockless form. It has a syntax *mostly* compatible with the
now deprecated `Ember.SelectView` which makes transitioning your
applications a bit easier.

If you can, use vanilla `x-select`. If you must, use `x-select-blockless`.

## Basic Example

```handlebars
{{x-select action="tagYouAreIt" disabled=isDisabled
  multiple=true
  content=folks
  value=it
  optionValuePath="content.id"
  optionLabelPath="content.name"}}
```
**A note about selection vs. value**  
When using Ember.Select, one would set either the **value** or **selection** property in order to bind a selected option to a property.  X-Select departs from Ember.Select and does not support the **selection** option.  Instead, only use the **value** option when binding to properties.


## EmberX

emberx-select-blockless is part of the "missing components of ember" collectively
known as emberx. See also:

* [emberx-select](https://github.com/thefrontside/emberx-select)
* [emberx-slider](https://github.com/thefrontside/emberx-slider)
* [emberx-files](https://github.com/thefrontside/emberx-files)

## Installation

```
ember install emberx-select-blockless
```

## Running Tests

* `ember test`
* `ember test --server`
