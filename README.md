
# Getting started

A fast, reliable, and modular Go implementation of an ERC-4337 Bundler.


# Contributing

## Prerequisites

- Go 1.20 or later
- Access to a node with `debug` API enabled for custom tracing.

## Setup

```bash
# Installs https://github.com/cosmtrek/air for live reloading.
# Runs go mod tidy.
make install-dev

# Generates base .env file.
# All variables in this file are required and should be filled.
# Running this command WILL override current .env file.
make generate-environment

# Parses private key in .env file and prints public key and address.
make fetch-wallet
```

## Run bundler in `private` mode

Start a local bundler instance:

```bash
make dev-private-mode
```

If you need to reset the embedded database:

```bash
# This will delete the default data directory at /tmp/stackup_bundler
make dev-reset-default-data-dir
```

# License

Distributed under the GPL-3.0 License. See [LICENSE](./LICENSE) for more information.
