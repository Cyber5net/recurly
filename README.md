<a href="https://heroku.com/deploy"><img align="right" src="https://www.herokucdn.com/deploy/button.png"></a>
Recurly.js examples
===================
<p align="center">
  <img src="http://i.imgur.com/hu8hAqs.png" align="center">
</p>

This repository contains a set of example implementations of
[recurly.js][recurly-js] using html, css, and JavaScript, and a set of API usage
examples to demonstrate a few common use-cases for collecting and using
recurly.js tokens.

Please note that these examples are not meant to be set onto a web server and
forgotten. They are intended to act as a suggestion, wherein your custom needs
may fill in any implementaiton gaps.

### Deploy to Heroku

This repository can be deployed immediately to Heroku using the included [Ruby Heroku API backend](api/ruby-heroku).
If you choose to do this, feel free to delete the other language backends from your clone.

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

### Payment form examples

- [Payment form examples][examples]

### API token usage examples

- [Ruby](api/ruby)
- [Ruby on Heroku](api/ruby-heroku)
- [Node](api/node)
- [Python](api/python)
- [PHP](api/php)
- [Java](api/java)

### Running locally

These examples are meant to be run locally, allowing you to easily experiment with
modifications and get running quickly.

Simply clone this repository, read through the simple application code to
familiarize yourself, and follow the startup instructions in one of the [API
token usage examples](api) above.

You'll want to adjust the code to fit your specific redirection and error
handling needs, but the example applications are designed to perform essential
API functions on first boot.

**Note**: These examples are purely for demonstration purposes and we do not recommend
using them as the foundation of a production system.

#### Configuring the examples

Each API example will pull configuration values from environment variables. You may set
them to quickly configure the example to connect to your Recurly site.

| Environment variable | description |
| -------------------- | ----------- |
| RECURLY_SUBDOMAIN | The subdomain of your recurly site |
| RECURLY_API_KEY | Your [private API key][api-keys] |
| RECURLY_PUBLIC_KEY | Your [public API key][api-keys] |
| SUCCESS_URL | A URL to redirect to when an action suceeds |
| ERROR_URL | A URL to redirect to when an error occurs |

### Contributing

[See CONTRIBUTING file](CONTRIBUTING.md).

### License

[MIT](license.md)

[recurly-js]: https://github.com/recurly/recurly-js
[examples]: public
[api-keys]: https://app.recurly.com/go/integrations/api_keys
