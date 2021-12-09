This repository contains the demos for the [*Defending against XSS with CSP*](https://auth0.com/blog/defending-against-xss-with-csp) blog post at Auth0. 

## About the demo

The demo is implemented as a single NodeJS Express server running on localhost. Each of the CSP scenarios is implemented in a different endpoint.

Note that the demo uses Express and the [express-csp-header](https://www.npmjs.com/package/express-csp-header) middleware to configure CSP policies. This middleware mostly offers syntactic sugar to define a CSP header in a more straightforward way. The middleware will send a proper `Content-Security-Policy` header on the response, as you can observe in the browser's developer tools.

Other languages and frameworks likely support similar libraries or middleware packages.


## Running the demo

Follow these steps to run the demo:

* `npm install`
* `node index.js`
* Opening [http://localhost:3000](http://localhost:3000) should give you a page saying "Welcome to this CSP demo. Try one of the demo endpoints"
