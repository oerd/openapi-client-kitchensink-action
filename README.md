# A Github Action for OpenAPI consumers

Generates client code and documentation from OpenAPI specs and publishes them.

## Motivation

There are a number of common steps that you go through when working with OpenAPI specs.

| Feature | Status |
| ------- | ------ |
| Generating clients for specific languages | ❌ |
| Publishing clients in package registries | ❌ |
| Generating and publishing API documentation | ❌ |
| Running contract-based tests on the clients | ❌ |

All these steps are usually run as part of the CI/CD pipelines. Wrapping these in a single action
will reduce code repetition and simplify engineering the pipelines.

An additional benefit is the reduced effort to propagate new functionality to multiple repositories
using this action. Just like with software libraries, the upgrade effort is constrained to reading
the Changelog and adding/updating the required input values.

### Feature statuses

✅ - Completely implemented
⏳ - Partially implemented
❌ - Not implemented
