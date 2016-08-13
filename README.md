# Meteor-UI5
This package is a work in progress for using UI5 with Meteor.  It contains
a new UI5 model for reactively binding meteor collections and queries to
UI5 controls.  It does not include the OpenUI5 library itself which has to be bootstrapped via a script element in HTML in the normal manner.

**WARNING:** This software is in an early beta state. `0.x` point releases may contain breaking changes.

## Using this package
This package can be added to your meteor project with ```meteor add propellerlabsio:meteor-ui5```.

Please see the [Meteor Ui5 website](http://meteor-ui5.propellerlabs.io) for documentation and demos of all of the features of this package. In particular, the following resources might be useful:
* [Quickstart guide](http://meteor-ui5.propellerlabs.io/#/docs/quickstart)
* [Tutorial](http://meteor-ui5.propellerlabs.io/#/tutorial)

## Building
1. After cloning the repo, run `npm install` to install build dependencies.
1. Run `npm run-script build` after making any changes to files in the `src/` directory. This will rebuild the `dist/` files and the documentation.  Meteor's own build tool will handle everything after that.

## Roadmap

This is the roadmap for the `meteor-ui5` package:

### v0.1 - This version currently under construction

1. Clean up & complete jsdoc comments in all code.
1. Add license files and headers.

### v0.2+

1. Add multifilter support (where single filter object is itself an array of filters with and/or conditions defined between them).
1. Filtering/sorting on list binding to array properties of single documents.
1. Add support for two-way binding (requires allow write to collections - not Meteor best practice which is update via method).
1. Add support for paging.  UI5 instantiates multiple control objects for every record in a list.  Need to limit the amount of front-end memory consumed when paging through large lists.
1. Incorporate UI5 webapp into meteor build process.
1. Build Meteor UI5 version of accounts-ui for integration with unified shell.

### Maybe

1. Add TreeBinding model

## License
This software is licensed under the Apache License, Version 2.0 - see LICENSE.txt
