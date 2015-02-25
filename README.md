# Spacing

The Predix Experience Spacing module is a small collection of helper classes for spacings like margin and padding. This module is a fork of inuitcss' [spacing](https://github.com/inuitcss/trumps.spacing) module.

## Dependencies

Px's Spacing Responsive module depends on two other Px and inuitcss modules:

* [settings.defaults](https://github.com/inuitcss/settings.defaults)
* [px-functions-design](https://github.sw.ge.com/pxc/px-functions-design)

## Installation

Install this module and its dependencies using bower:

    bower install --save https://github.sw.ge.com/pxc/px-spacing-design.git

Once installed, `@import` into your project's Sass file in its Trumps layer:

    @import "px-spacing-design/sass/trumps.spacing";

## Import once

All rulesets are wrapped in the following `@if` statement:

    @if import-once('trumps.spacing') { ... }

## Usage

These flags are available and, if needed, should be set to `true` prior to importing the module:

    $inuit-enable-margins
    $inuit-enable-margins--tiny
    $inuit-enable-margins--small
    $inuit-enable-margins--large
    $inuit-enable-margins--huge
    
    $inuit-enable-margins--negative
    $inuit-enable-margins--negative-tiny
    $inuit-enable-margins--negative-small
    $inuit-enable-margins--negative-large
    $inuit-enable-margins--negative-huge
    
    $inuit-enable-margins--none
    
    $inuit-enable-paddings
    $inuit-enable-paddings--tiny
    $inuit-enable-paddings--small
    $inuit-enable-paddings--large
    $inuit-enable-paddings--huge
    
    $inuit-enable-paddings--none

The following dimension variables can be customized:

    $inuit-margin
    $inuit-padding

The conventions used in the classes in the spacing module are as follows:

    .[negative][type][direction][size] {}

E.g.:

* `.-mt+` will give you a large (`+`) negative (`-`) margin (`m`) top (`t`).
* `.p--` will give you a tiny (`--`) padding (`p`).
* `.mh++` will give you a huge (`++`) horizontal (`h`) margin (`m`).
* `.mb0` will give you no (`0`) margin (`m`) bottom (`b`).
* `.pl-` will give you a small (`-`) padding (`p`) left (`l`).

Knowing these conventions means you can compose a huge array of spacing helpers.

## Options

These classes are available if the following variable flags are set to `true`:

`$inuit-enable-margins`:

* `m`: add default margins to all sides
* `mt`: add default margin top
* `mr`: add default margin right
* `mb`: add default margin bottom
* `ml`: add default margin left
* `mh`: add default margins right and left
* `mv`: add default margins top and bottom

`$inuit-enable-margins--tiny`:

* `m--`: add tiny margins to all sides
* `mt--`: add tiny margin top
* `mr--`: add tiny margin right
* `mb--`: add tiny margin bottom
* `ml--`: add tiny margin left
* `mh--`: add tiny margins right and left
* `mv--`: add tiny margins top and bottom

`$inuit-enable-margins--small`:

* `m-`: add small margins to all sides
* `mt-`: add small margin top
* `mr-`: add small margin right
* `mb-`: add small margin bottom
* `ml-`: add small margin left
* `mh-`: add small margins right and left
* `mv-`: add small margins top and bottom

`$inuit-enable-margins--large`:

* `m+`: add large margins to all sides
* `mt+`: add large margin top
* `mr+`: add large margin right
* `mb+`: add large margin bottom
* `ml+`: add large margin left
* `mh+`: add large margins right and left
* `mv+`: add large margins top and bottom

`$inuit-enable-margins--huge`:

* `m++`: add huge margins to all sides
* `mt++`: add huge margin top
* `mr++`: add huge margin right
* `mb++`: add huge margin bottom
* `ml++`: add huge margin left
* `mh++`: add huge margins right and left
* `mv++`: add huge margins top and bottom

`$inuit-enable-margins--negative`:

* `-m`: add default negative margins to all sides
* `-mt`: add default negative margin top
* `-mr`: add default negative margin right
* `-mb`: add default negative margin bottom
* `-ml`: add default negative margin left
* `-mh`: add default negative margins right and left
* `-mv`: add default negative margins top and bottom

`$inuit-enable-margins--negative-tiny`:

* `-m--`: add tiny negative margins to all sides
* `-mt--`: add tiny negative margin top
* `-mr--`: add tiny negative margin right
* `-mb--`: add tiny negative margin bottom
* `-ml--`: add tiny negative margin left
* `-mh--`: add tiny negative margins right and left
* `-mv--`: add tiny negative margins top and bottom

`$inuit-enable-margins--negative-small`:

* `-m-`: add small negative margins to all sides
* `-mt-`: add small negative margin top
* `-mr-`: add small negative margin right
* `-mb-`: add small negative margin bottom
* `-ml-`: add small negative margin left
* `-mh-`: add small negative margins right and left
* `-mv-`: add small negative margins top and bottom

`$inuit-enable-margins--negative-large`:

* `-m+`: add large negative margins to all sides
* `-mt+`: add large negative margin top
* `-mr+`: add large negative margin right
* `-mb+`: add large negative margin bottom
* `-ml+`: add large negative margin left
* `-mh+`: add large negative margins right and left
* `-mv+`: add large negative margins top and bottom

`$inuit-enable-margins--negative-huge`:

* `-m++`: add huge negative margins to all sides
* `-mt++`: add huge negative margin top
* `-mr++`: add huge negative margin right
* `-mb++`: add huge negative margin bottom
* `-ml++`: add huge negative margin left
* `-mh++`: add huge negative margins right and left
* `-mv++`: add huge negative margins top and bottom

`$inuit-enable-margins--none`:

* `m0`: remove margins
* `mt0`: remove margin top
* `mr0`: remove margin right
* `mb0`: remove margin bottom
* `ml0`: remove margin left
* `mh0`: remove margins right and left
* `mv0`: remove margins top and bottom

`$inuit-enable-paddings`:

* `p`: add default padding to all sides
* `pt`: add default padding top
* `pr`: add default padding right
* `pb`: add default padding bottom
* `pl`: add default padding left
* `ph`: add default padding right and left
* `pv`: add default padding top and bottom

`$inuit-enable-paddings--tiny`:

* `p--`: add tiny padding to all sides
* `pt--`: add tiny padding top
* `pr--`: add tiny padding right
* `pb--`: add tiny padding bottom
* `pl--`: add tiny padding left
* `ph--`: add tiny padding right and left
* `pv--`: add tiny padding top and bottom

`$inuit-enable-paddings--small`:

* `p-`: add small padding to all sides
* `pt-`: add small padding top
* `pr-`: add small padding right
* `pb-`: add small padding bottom
* `pl-`: add small padding left
* `ph-`: add small padding right and left
* `pv-`: add small padding top and bottom

`$inuit-enable-paddings--large`:

* `p+`: add large padding to all sides
* `pt+`: add large padding top
* `pr+`: add large padding right
* `pb+`: add large padding bottom
* `pl+`: add large padding left
* `ph+`: add large padding right and left
* `pv+`: add large padding top and bottom

`$inuit-enable-paddings--huge`:

* `p++`: add huge padding to all sides
* `pt++`: add huge padding top
* `pr++`: add huge padding right
* `pb++`: add huge padding bottom
* `pl++`: add huge padding left
* `ph++`: add huge padding right and left
* `pv++`: add huge padding top and bottom

`$inuit-enable-paddings--none`:

* `p0`: remove padding
* `pt0`: remove padding top
* `pr0`: remove padding right
* `pb0`: remove padding bottom
* `pl0`: remove padding left
* `ph0`: remove padding right and left
* `pv0`: remove padding top and bottom

