# crystalize-promise

## Global default Promise implementation for crystalize modules
   by crystalize.

All crystalize modules that reference promises use this module. This module
allows the user to swap out the default `Promise` implementation for one their
preference. It defaults to ES6 Promises.

For example, to change the default Promise implementation to `bluebird`, simply
do the following:

     require("crystalize-promise").Promise = require("bluebird");
