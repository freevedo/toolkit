# Overleaf Toolkit

This repository contains the Overleaf Toolkit, the standard tools for running a local
instance of [Overleaf](https://overleaf.com). This toolkit will help you to set up and administer both Overleaf Community Edition (free to use, and community supported), and Overleaf Server Pro (commercial, with professional support).

The [Developer wiki](https://github.com/overleaf/overleaf/wiki) contains further documentation on releases, features and other configuration elements.


## Getting Started

Clone this repository locally:

``` sh
git clone https://github.com/overleaf/toolkit.git ./overleaf-toolkit
```

Then follow the [Quick Start Guide](./doc/quick-start-guide.md).


## Documentation

See [Documentation Index](./doc/README.md)


## Contributing

See the [CONTRIBUTING](https://github.com/overleaf/overleaf/blob/main/CONTRIBUTING.md) file.


## Getting Help

Users of the free Community Edition should [open an issue on github](https://github.com/overleaf/toolkit/issues). 

Users of Server Pro should contact `support@overleaf.com` for assistance.

In both cases, it is a good idea to include the output of the `bin/doctor` script in your message.


## Mac OS considerations

- please install coreutils and gnu-tar via homebrew:

```sh
brew install coreutils gnu-tar
```
- This code has been updated to work with arm macs. The docker-compose file has been updated to use the `linux/amd64` platform. If you are using an arm mac, you may need to add `platform: linux/arm64` to the docker-compose file for the services that are not working.