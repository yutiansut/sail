+++
type="docs"
title="Getting Started"
browser_title="Sail - Docs - Getting Started"
section_order=1
+++

## Platform Support

Currently Sail supports both Linux and MacOS. Windows support is planned for a future release.

## Host Dependencies

Before using Sail, there are several dependencies that must be installed on the host system:

- [Docker](https://docs.docker.com/install/)
- [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [Chrome](https://www.google.com/chrome/) or [Chromium](https://www.chromium.org/getting-involved/download-chromium) - not required, but strongly recommended for best [code-server](https://github.com/codercom/code-server) support.


## Installation

### Stable Releases

Binary releases can be downloaded from our [GitHub.](https://github.com/codercom/sail/releases)

### From Source

To install the latest version of `sail`, run:

```bash
go install go.coder.com/sail
```

_`go install` will install to `$GOPATH/bin`_


### Verifying the Installation

To verify Sail is properly installed, run `sail --help` on your system. If everything is installed
properly, you should see Sail's help text.

```bash
sail --help
```


## Updating

To gracefully update `sail`, simply overwrite the binary with the binary 
in the new release.

If you installed via `go install`, just run the same command again.