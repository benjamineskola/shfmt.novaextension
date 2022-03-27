# Shfmt Nova Extension

It’s a stand-alone Nova extension to use [Shfmt](https://github.com/mvdan/sh),
based on [Aeron](https://github.com/Aeron/)'s
[Black extension](https://github.com/Aeron/Black.novaextension).

## Requirements

Before using the extension, it’s necessary to install Shfmt itself if you
haven't already.

Shfmt can be installed simply by running `brew install shfmt`.

## Configuration

The extension supports both global and workspace configurations. A workspace
configuration always overrides a global one.

### Options

There are three extension options available to configure: executable path,
command arguments, and format on save. By default, the executable path is
`/usr/local/bin/shfmt`, with no additional arguments, and formatting on saving
is on.

There are also a number of formatting options to configure: indentation size,
POSIX compatibility, and simplification mode. All of these default to the Shfmt
defaults: tab indentation, Bash compatibility, no simplification.

Other options can be set using the command arguments option, which will override
the others in case of a conflict.

## Credits

The bulk of the code is from [Aeron](https://github.com/Aeron/)'s
[Black extension](https://github.com/Aeron/Black.novaextension). All I've done
is swap out the executable for [Shfmt](https://github.com/mvdan/sh). The
extension logo is from
[nova-shellcheck](https://github.com/olly/nova-shellcheck) and is
[MIT licenced](https://github.com/olly/nova-shellcheck/blob/main/LICENSE).
