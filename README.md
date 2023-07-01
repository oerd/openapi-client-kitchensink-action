# A Github Action for OpenAPI consumers

Generates client code and documentation from OpenAPI specs and publishes them.

## Motivation

There are a number of common steps that you go through when working with OpenAPI specs.

All these steps are usually run as part of the CI/CD pipelines. Wrapping these in a single action
will reduce code repetition and simplify engineering the pipelines.

An additional benefit is the reduced effort to propagate new functionality to multiple repositories
using this action. Just like with software libraries, the upgrade effort is constrained to reading
the Changelog and adding/updating the required input values.

## Features

The following is a list of features that have been identified for inclusion in this actions'
roadmap. The order is indicative of their importance, but does not necessarily match the order
in which work will be prioritized for their implementation.

| Feature | Status |
| ------- | ------ |
| Generating clients for specific languages | ❌ |
| Publishing clients in package registries | ❌ |
| Generating and publishing API documentation | ❌ |
| Running contract-based tests on the clients | ❌ |

> ⚠️ _Note:_
>
> It is not yet clear if the best implementation of this reusable functionality
> is via a _composite action_ or a _reusable workflow_. Part of the planned
> work includes exploring what's best (probably a mix between the two).

### Feature statuses

Feature status icons have the following meanings:

* ✅ - Implemented
* ⏳ - Partially implemented
* ❌ - Not implemented
