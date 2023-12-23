## README

This repository defines a devcontainer for getting started with Theia development. It satisfies the baseline requirements for taking the official Theia tutorial:

**Build your own IDE/Tool**.

See the references section below for more information.

### Notes

Theia dependencies include:

* [node-keytar](https://github.com/atom/node-keytar#on-linux), and,
* [node-native-keymap](xhttps://github.com/Microsoft/node-native-keymap)

This means additional dependencies not included in the base devcontainer must be installed on the host system. To remedy this, the current repository includes a Dockerfile that extends the base devcontainer and installs the required packages.

## References

[Getting Started/Composing Applications](https://theia-ide.org/docs/composing_applications)