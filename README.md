<div align="center">
  <a href="https://www.pokt.network">
    <img src="pocket-core.png" alt="Pocket Network logo" width="340"/>
  </a>
</div>

# Pocket Core <!-- omit in toc -->

Official golang implementation of the Pocket Network Protocol.

<div>
  <a href="https://godoc.org/github.com/pokt-network/pocket-core"><img src="https://img.shields.io/badge/godoc-reference-blue.svg"/></a>
  <a href="https://goreportcard.com/report/github.com/pokt-network/pocket-core"><img src="https://goreportcard.com/badge/github.com/pokt-network/pocket-core"/></a>
  <a href="https://golang.org"><img  src="https://img.shields.io/badge/golang-v1.18-red.svg"/></a>
  <a href="https://github.com/tools/godep" ><img src="https://img.shields.io/badge/godep-dependency-71a3d9.svg"/></a>
</div>

## Overview

<div>
    <a href="https://discord.gg/pokt"><img src="https://img.shields.io/discord/553741558869131266"></a>
    <a  href="https://github.com/pokt-network/pocket-core/releases"><img src="https://img.shields.io/github/release-pre/pokt-network/pocket-core.svg"/></a>
    <a href="https://circleci.com/gh/pokt-network/pocket-core"><img src="https://circleci.com/gh/pokt-network/pocket-core.svg?style=svg"/></a>
    <a  href="https://github.com/pokt-network/pocket-core/pulse"><img src="https://img.shields.io/github/contributors/pokt-network/pocket-core.svg"/></a>
    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg"/></a>
    <!--<a href="https://github.com/pokt-network/pocket-core/pulse"><img src="https://img.shields.io/github/last-commit/pokt-network/pocket-core.svg"/></a>-->
    <a href="https://github.com/pokt-network/pocket-core/pulls"><img src="https://img.shields.io/github/issues-pr/pokt-network/pocket-core.svg"/></a>
    <a href="https://github.com/pokt-network/pocket-core/releases"><img src="https://img.shields.io/badge/platform-linux%20%7C%20macos-pink.svg"/></a>
    <!--<a href="https://github.com/pokt-network/pocket-core/issues"><img src="https://img.shields.io/github/issues-closed/pokt-network/pocket-core.svg"/></a>-->
</div>

The Pocket Core application will allow anyone to spin up a Pocket Network full node, with options to enable/disable functionality and modules according to each deployment. For more information on Pocket Network, visit [pokt.network](https://pokt.network).

## Table of Contents <!-- omit in toc -->

- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Documentation](#documentation)
- [Database Snapshots](#database-snapshots)
- [Accessing TestNet](#accessing-testnet)
- [Running the tests](#running-the-tests)
- [Contributing](#contributing)
- [MainNet Seeds](#mainnet-seeds)
- [Support \& Contact](#support--contact)
- [License](#license)

## Installation

Clone the repository, `cd` into it and run `go build app/cmd/pocket_core/pocket.go`.
> Be sure to add the `pocket` executable to your `PATH` if you'd like to use it without direct reference to the binary.

## Usage

To run the Pocket Core binary you can use the following flags alongside the `pocket` executable:

```bash
Usage:
  pocket [command]

Available Commands:
  accounts    account management
  apps        application management
  completion  Generate the autocompletion script for the specified shell
  gov         governance management
  help        Help about any command
  nodes       node management
  query       query the blockchain
  reset       Reset pocket-core
  start       starts pocket-core daemon
  stop        Stop pocket-core
  util        utility functions
  version     Get current version

Flags:
      --datadir string            data directory (default is $HOME/.pocket/
  -h, --help                      help for pocket
      --node string               takes a remote endpoint in the form <protocol>://<host>:<port>
      --persistent_peers string   a comma separated list of PeerURLs: '<ID>@<IP>:<PORT>,<ID2>@<IP2>:<PORT>...<IDn>@<IPn>:<PORT>'
      --remoteCLIURL string       takes a remote endpoint in the form of <protocol>://<host> (uses RPC Port)
      --seeds string              a comma separated list of PeerURLs: '<ID>@<IP>:<PORT>,<ID2>@<IP2>:<PORT>...<IDn>@<IPn>:<PORT>'

Use "pocket [command] --help" for more information about a command.
```

For more detailed command information, see the [usage section](doc/specs/cli/).

## Documentation

[Visit our user documentation](https://docs.pokt.network) for tutorials and technical information on the Pocket Network.

## Database Snapshots

Snapshots are provided by [Liquify LTD](https://www.liquify.io/) details on how to access the snapshots can be found in [snapshot.md](doc/guides/snapshot.md)

## Pocket Pruner

An offline pruning tool is provided by [C0D3R](https://c0d3r.org/). The tool is available in [their GitHub repository](https://github.com/msmania/pocket-pruner/).

## Accessing TestNet

TestNet information can be found at [testnet.md](doc/guide/testnet.md)

## Running the tests

To run the Pocket Core unit tests, `go test -short -v -p 1 ./...`

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on contributions and the process of submitting pull requests.

## MainNet Seeds

MainNet seeds are being maintained by [NodeFleet](https://nodefleet.org/) and more details can be found at [docs.pokt.network/node/seeds/](https://docs.pokt.network/node/seeds/).

## Support & Contact

<div>
  <a  href="https://twitter.com/poktnetwork" ><img src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social"></a>
  <a href="https://t.me/POKTnetwork"><img src="https://img.shields.io/badge/Telegram-blue.svg"></a>
  <a href="https://www.facebook.com/POKTnetwork" ><img src="https://img.shields.io/badge/Facebook-red.svg"></a>
  <a href="https://research.pokt.network"><img src="https://img.shields.io/discourse/https/research.pokt.network/posts.svg"></a>
</div>

## License

This project is licensed under the MIT License; see the [LICENSE.md](LICENSE.md) file for details
