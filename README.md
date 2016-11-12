# fcoo-modernizr

[Modernizr]: https://modernizr.com/
[modernizr-device]: https://github.com/FCOO/modernizr-device
[modernizr-mediaquery]: https://github.com/FCOO/modernizr-mediaquery
[grunt-modernizr]: https://github.com/Modernizr/grunt-modernizr

## Description
The Modernizr tests for FCOO applications

## Installation
### bower
`bower install https://github.com/FCOO/fcoo-modernizr.git --save`

## Demo

A full list of added [Modernizr] tests can be seen at 
http://FCOO.github.io/fcoo-modernizr/demo/ 

A full list of **available** [Modernizr] tests can be seen at 
http://FCOO.github.io/fcoo-modernizr/demo/list.html

## Modernizr
### Installation 
To edit this packages you need to install modernizr by running

	npm install -g modernizr

### Create
The [Modernizr] JavaScript file for this package is created when running one of the following grunt-commands:

	>grunt dev 
	>grunt prod
	>grunt push

### Tests
The following Modernizr tests are included

    fullscreen-api
    touchevents
    chunit
    flexbox
    flexboxlegacy
    flexboxtweener
    flexwrap
    pointerevents
    remuni
         
### Edit/modify
To modify the options or features included you need to 

- edit the config-file `\src\modernizr-config.json`, OR
- go to [Modernizr Download](https://modernizr.com/download) and
	- Select the options and feature
	- Press the `BUILD` button and `download` the `Command Line Config` into `\src\modernizr-config.json`  

At [Modernizr Download](https://modernizr.com/download) and in `\src\modernizr-config.json` the settings are divided in *options* and *feature-detects* where 
**options** defines witch JavaScript methods are included. See [Modernizr API](https://modernizr.com/docs/#modernizr-api) for details.
**feature-detects** defines witch *browser feature* Modernizr will test for. 

### CSS Classes
The option *Add CSS Classes* at [Modernizr Download](https://modernizr.com/download) must be selected or `options: [..]` must include `"setClasses"`. 
Then each test in `feature-detects` will set a class to `<html>` to mark the result of the test: `<html class="TEST">` or `<html class="no-TEST">`

**Example:** The test *Event Listener* will detects native support for addEventListener and set the class `eventlistener` or `no-eventlistener` to `<html>`

### options

See [Modernizr API](https://modernizr.com/docs/#modernizr-api) for description of the different methods.
The following methods must always be included:

	Modernizr.addTest()
	Modernizr.atRule()
	Modernizr.hasEvent()
	Modernizr.mq()

`html5printshiv` and `html5shiv` are polyfills for browsers not supporting HTML5  

#### NOTE
The option `minify` **MUST** be set to **`false`**
The option `Add CSS Classes` **MUST** be set to **`true`**

### feature-detects
See [Modernizr - Features detected by Modernizr](https://modernizr.com/docs#features) for a complete list of possible tests

See complete meta-data file at http://FCOO.github.io/fcoo-modernizr/src/fcoo-modernizr-metadata.json
 
A full list of **added** [Modernizr] tests can be seen at [the demo page](http://FCOO.github.io/fcoo-modernizr/demo/)

A full list of **available** [Modernizr] tests can be seen [here](http://FCOO.github.io/fcoo-modernizr/demo/list.html)



## Copyright and License
This plugin is licensed under the [MIT license](https://github.com/FCOO/fcoo-modernizr/LICENSE).

Copyright (c) 2016 [FCOO](https://github.com/FCOO)

## Contact information

NielsHolt nho@fcoo.dk


## Credits and acknowledgements
