<div align="center">

# asdf-tuist [![Build](https://github.com/tuist/asdf-tuist/actions/workflows/build.yml/badge.svg)](https://github.com/tuist/asdf-tuist/actions/workflows/build.yml) [![Lint](https://github.com/tuist/asdf-tuist/actions/workflows/lint.yml/badge.svg)](https://github.com/tuist/asdf-tuist/actions/workflows/lint.yml)

[tuist](https://docs.tuist.io) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

# Dependencies

- `bash`, `curl`, `tar`, and [POSIX utilities](https://pubs.opengroup.org/onlinepubs/9699919799/idx/utilities.html).

# Install

Plugin:

```shell
asdf plugin add tuist
# or
asdf plugin add tuist https://github.com/tuist/asdf-tuist.git
```

tuist:

```shell
# Show all installable versions
asdf list-all tuist

# Install specific version
asdf install tuist latest

# Set a version globally (on your ~/.tool-versions file)
asdf global tuist latest

# Now tuist commands are available
tuist --help
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

# Configuration

## Custom Installation URL

You can override the default GitHub repository URL by setting the `MISE_TUIST_INSTALL_URL` environment variable. This is useful if you want to install tuist from a fork or a custom mirror.

```shell
# Set custom installation URL
export MISE_TUIST_INSTALL_URL="https://github.com/your-org/tuist"

# Install tuist from the custom URL
asdf install tuist latest

```

If `MISE_TUIST_INSTALL_URL` is not set, the plugin will use the default repository: `https://github.com/tuist/tuist`

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/tuist/asdf-tuist/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [Tuist](https://github.com/tuist/)
