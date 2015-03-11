# simple-http

A simple wrapper for making an http get request to a JSON endpoint in Node.js. Includes the ability to set a timeout.

``` js
var simpleHttp = require('simple-http');

simpleHttp.getJson('http://localhost/api', function(err, response) {
	console.log(response);      
});
```

## Using Timeout

``` js
var simpleHttp = require('simple-http');
var timeoutInMilliSeconds = 2000;

simpleHttp.getJson('http://localhost/api', timeoutInMilliSeconds, function(err, response) {
	console.log(response);      
});
```