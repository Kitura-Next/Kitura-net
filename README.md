<p align="center">
<a href="http://kituranext.org/">
<img src="https://raw.githubusercontent.com/Kitura-Next/Kitura/master/Sources/Kitura/resources/kitura-bird.svg?sanitize=true" height="100" alt="Kitura">
</a>
</p>

<p align="center">
    <a href="https://www.kituranext.org/learn/">
    <img src="https://img.shields.io/badge/docs-kitura-1FBCE4.svg" alt="APIDoc"></a>
    <a href="https://github.com/Kitura-Next/Kitura-net/actions?query=workflow%3ASwift+MacOS">
    <img src="https://github.com/Kitura-Next/Kitura-net/workflows/Swift%20MacOS/badge.svg"></a>
    <a href="https://github.com/Kitura-Next/Kitura-net/actions?query=workflow%3ASwift+Ubuntu">
    <img src="https://github.com/Kitura-Next/Kitura-net/workflows/Swift%20Ubuntu/badge.svg"></a>
    <img src="https://img.shields.io/badge/license-Apache2-blue.svg?style=flat" alt="Apache 2">
    <a href="http://swift-at-ibm-slack.mybluemix.net/">
    <img src="http://swift-at-ibm-slack.mybluemix.net/badge.svg" alt="Slack Status"></a>
</p>

# Kitura-Net

The Kitura-net module contains logic for sending and receiving HTTP requests. It also contains the structure for listening on a port and sending requests to a delegate for processing. It can be used to create HTTP/CGI servers on specific ports, and provides HTTP functionality.

We expect most of our users to require higher level concepts such as routing, templates and middleware, these are not provided in Kitura-net, if you want to use those facilities you should be coding at the Kitura level, for this please see the [Kitura](https://github.com/Kitura-Next/Kitura) project. Kitura-net underpins Kitura which offers a higher abstraction level to users.

Kitura-net utilises the [BlueSocket](https://github.com/Kitura-Next/BlueSocket) framework, the [BlueSSLService](https://github.com/Kitura-Next/BlueSSLService.git) framework and [CCurl](https://github.com/Kitura-Next/CCurl.git).

## Features

- Port Listening
- FastCGI Server support
- HTTP Server support (request and response)

## Usage

#### Add dependencies

Add the `Kitura-net` package to the dependencies within your application’s `Package.swift` file. Substitute `"x.x.x"` with the latest `Kitura-net` [release](https://github.com/Kitura-Next/Kitura-net/releases).

```swift
.package(url: "https://github.com/Kitura-Next/Kitura-net.git", from: "x.x.x")
```

Add `KituraNet` to your target's dependencies:

```swift
.target(name: "example", dependencies: ["KituraNet"]),
```

#### Import package

  ```swift
  import KituraNet
  ```

## Contributing to Kitura-net

All improvements to Kitura-net are very welcome! Here's how to get started with developing Kitura-net itself.

1. Clone this repository.

`$ git clone https://github.com/Kitura-Next/Kitura-net && cd Kitura-net`

2. Build and run tests.

`$ swift test`

You can find more info on contributing to Kitura in our [contributing guidelines](https://github.com/Kitura-Next/Kitura/blob/master/.github/CONTRIBUTING.md).
## Swift version
Requires **Swift 5.1** or newer. You can download this version of the Swift binaries by following this [link](https://swift.org/download/). Compatibility with other Swift versions is not guaranteed.
## API Documentation
For more information visit our [API reference](https://kitura-next.github.io/Kitura-net/index.html).

## Community

We love to talk server-side Swift, and Kitura. Join our [Slack](http://slack.kituranext.org/) to meet the team!

## License
This library is licensed under Apache 2.0. Full license text is available in [LICENSE](https://github.com/Kitura-Next/Kitura-net/blob/master/LICENSE.txt).
