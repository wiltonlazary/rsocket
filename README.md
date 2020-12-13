# RSocket Protocol

RSocket is an application protocol providing [Reactive Streams](http://www.reactive-streams.org) semantics over an asynchronous, binary boundary.

It enables the following symmetric interaction models via async message passing over a single connection:

- request/response (stream of 1)
- request/stream (finite/infinite stream of many)
- fire-and-forget (no response)
- channel (bi-directional streams)

It also supports connection resumption to allow resuming long-lived streams across different transport connections. This is particularly useful for mobile<->server communication when network connections drop, switch, and reconnect frequently.

Artifacts include:

- [RSocket Protocol](Protocol.md)
- Protocol Extensions
  - [Well-known MIME Types](Extensions/WellKnownMimeTypes.md)
  - [Stream Data MIME Types Definition](Extensions/PerStreamDataMimeTypesDefinition.md)
  - [Composite Metadata](Extensions/CompositeMetadata.md)
  - [Routing](Extensions/Routing.md)
  - [Tracing (Zipkin)](Extensions/Tracing-Zipkin.md)
  - [Authentication](Extensions/Security/Authentication.md)
- [Motivation for creating this protocol](Motivations.md)
- [Frequently Asked Questions](FAQ.md)

More information and links to various implementations can be found at http://rsocket.io

## Bugs and Feedback

For bugs, questions and discussions please use the [Github Issues](https://github.com/rsocket/rsocket/issues).

## LICENSE

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

<http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
