# Changelog

# 0.4.0 - 2018-05-03

- Muti process support (new parameter to pass to the ProductionPluginRunner), disabled by default
- Improve Audience External Feed support (`getInstanceContext` helper)
- Better support of types with Instance properties fetching
- Some naming changes (see the migration seciton in `README`)\

# 0.3.9 - 2018-04-05

- Add an option to return a 429 HTTP code when the plugin is too busy

# 0.3.8 - 2018-03-19

- Fix invalid characters issues in the DisplayContext header

# 0.3.7 - 2018-03-13

- Add `creative_variant` on the `BidOptimizerPluginResponse` interface
- Add `compartment_id` on the `UserAccountIdentifierInfo` interface

# 0.3.6 - 2018-03-05

- Add `blast_id` on the `EmailRoutingRequest` interface
- Add `creative_variant` on the `AdRendererRequest` interface

# 0.3.5 - 2018-01-11

- Fix Audience Feed support (wrong initial integration which was not aligned with the API)
- Add an Helper to do the Handlebars macros mapping for AdRenderer with Templating using the Handlebars Engine
- Update IAS TAG integration for AdRenderer using the Handlebars engine (escape the media_id as it's passed in an IAS URL)

# 0.3.4 - 2018-01-09

- Fix overiding request options parameters in requestGatewayHelper

# 0.3.3 - 2018-01-05

- Add support for Audience Feed Connectors plugins

# 0.3.2 - 2017-12-15

- Remove a console.log in the handlebars engine

# 0.3.1 - 2017-12-01

- Improve error handling with async/await
- Fix error message of gateway helper
- Fix the JSON vs non JSON situations
- Add async middleware to stop using try catch in routes
- Add async middleware to all plugin routes
- Remove legacy log
- Update IAS Tag integration


# 0.3.0 - 2017-11-15

- New "Templating" support with AdRendererTemplatePlugin class (for AdRenderer that don't need recommendations)

# 0.2.4 - 2017-10-25

- Add support for email router and email renderer
- Fix User Activity Interface
- Add a MailJet Email router as an implementation example

## 0.2.3 - 2017-09-15

- Updated the UserActivityEventProperty Interface
- Fix some Activity Analyzer tests

## 0.2.2 - 2017-09-14

- Fix user_agent_id interface
- Add testing of User Agent id (case: null & check if correctly passed to recommender)

## 0.2.1 - 2017-09-13

- Added support of the BidOptimizer plugins
- Fix PluginProperty interface
- Added a BidOptimizer example
- Removed package-lock.json from examples for SDK release testing purposes
- Added some Geolocation helpers

## 0.2.0 - 2017-09-11

- Breaking changes in the SDK public API > Now relying on Javascript ES6 Class APIs. Not compatible with the 0.1.x versions of the SDK
- New interfaces for UserActivity / Recommendations objects
- New Plugin type to implement Ad Renderer using Recommendations and Templating features
- Handlebars.js template engine integration
- Testing capbility of plugin built with this SDK. See the examples to see how it works.
- SDK Tests: The SDK itself is now tested, you can run the tests by typing `npm test`
- Doc generation: Use `npm doc` to generate the documentation (using typedoc)

## 0.1.2 - 2017-08-08

- Fix missing value in ValueInterface (=> url)
- Fix log level case issue
- Add fetchDataFile helper (which return binary)
- Add custom InstanceContext builder use in Activity Analyzer example
- Fix error catching issue
- Exposed ActivityAnalyzer & ActivityAnalyzerProperty interfaces

## 0.1.1 - 2017-08-01

- Include the `build/` directory in the published package

## 0.1.0 - 2017-08-01

- Initial release
