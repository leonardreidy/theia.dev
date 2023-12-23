# README

This repository defines a devcontainer for getting started with Theia development. It satisfies the baseline requirements for taking the official Theia tutorial:

**Build your own IDE/Tool**.

See the references section below for more information.

## Prerequisites

It should be straightforward enough to use this repo with Docker Desktop or other similar utility. However, in order to use it to best advantage, it is recommended that you use [DevPod](https://devpod.sh/) or an equivalent. See the excellent [documentation](https://devpod.sh/docs/what-is-devpod) at the DevPod site for more information.

## Usage

To get started run the following commands:

```sh
# Install dependencies - and be patient, it takes awhile
yarn 

# Build
yarn build

# Start the application (with local plugins)
yarn theia start --plugins=local-dir:plugins
```

Now, open a new tab, and navigate to `http://localhost:3000` to see the application. If you encounter no issues at this point, then you have a working Theia development environment, and, as a nice bonus, a VSCode like IDE running in the browser that you can continue to customize.

## Notes

Theia dependencies include:

* [node-keytar](https://github.com/atom/node-keytar#on-linux), and,
* [node-native-keymap](https://github.com/Microsoft/node-native-keymap)

This means additional dependencies not included in the base devcontainer must be installed on the host system. To remedy this, the current repository includes a Dockerfile that extends the base devcontainer and installs the required packages.

## References

[DevPod/Getting Started/What is Devpod](https://devpod.sh/docs/what-is-devpod)

[Theia/Getting Started/Composing Applications](https://theia-ide.org/docs/composing_applications)