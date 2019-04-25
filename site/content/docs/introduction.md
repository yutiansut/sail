+++
type="docs"
title="Introduction"
browser_title="Sail - Docs  - Introduction"
section_order=0
+++


This site covers Sail's usage and concepts.

## What is Sail?

Sail is a CLI utility to manage Dockerized development environments. 
It uses the [docker](https://https://www.docker.com/) toolchain and [code-server](https://github.com/codercom/code-server) to create
reproducible, preconfigured, source controlled, and customizable development environments. 

## Why use Sail?

Sail is a completely new paradigm for development. Some of the key benefits for using Sail are:

1. **Source Controlled** - All project dependencies and configuration for a working development environment
   are explicitly set in your project's `.sail/Dockerfile`.
2. **Immutable Environments** - Projects are run inside of docker containers created from your project's `.sail/Dockerfile`
   to create a base development environment that is the same across all developers. If your environment
   gets messed up for any reason, just remove it and start with a clean slate.
3. **Quickly Contribute** - A project configured with Sail allows new developers to contribute extremely
   quickly since they don't have to worry about what dependencies or configuration they need to get
   a working environment.
4. **Bring Your Own Dotfiles** - Add your own environment configuration to any project you work on with a [hat](/docs/concepts/hats)
   so you can use your preferred shell or custom vim config.
5. **No Host Litter** - Easily experiment with new projects without having to litter your host system with
   project dependencies. All dependencies for sail projects are contained in the project's docker image. This
   also has the nice benefit of removing cross project dependency incompatibilities.


## How is it used?

```bash
# Develop sail within a sail container.
#
# This creates a docker container called `codercom_sail`,
# installs code-server in it, and opens the project in vscode.
sail run codercom/sail
```

See [Getting Started](/docs/getting-started) for installation instructions.
 