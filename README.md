oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![Downloads/week](https://img.shields.io/npm/dw/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/oclif/hello-world/blob/main/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g crawl-companies
$ crawl-companies COMMAND
running command...
$ crawl-companies (--version)
crawl-companies/0.0.0 darwin-arm64 node-v18.6.0
$ crawl-companies --help [COMMAND]
USAGE
  $ crawl-companies COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`crawl-companies hello PERSON`](#crawl-companies-hello-person)
* [`crawl-companies hello world`](#crawl-companies-hello-world)
* [`crawl-companies help [COMMAND]`](#crawl-companies-help-command)
* [`crawl-companies plugins`](#crawl-companies-plugins)
* [`crawl-companies plugins:install PLUGIN...`](#crawl-companies-pluginsinstall-plugin)
* [`crawl-companies plugins:inspect PLUGIN...`](#crawl-companies-pluginsinspect-plugin)
* [`crawl-companies plugins:install PLUGIN...`](#crawl-companies-pluginsinstall-plugin-1)
* [`crawl-companies plugins:link PLUGIN`](#crawl-companies-pluginslink-plugin)
* [`crawl-companies plugins:uninstall PLUGIN...`](#crawl-companies-pluginsuninstall-plugin)
* [`crawl-companies plugins:uninstall PLUGIN...`](#crawl-companies-pluginsuninstall-plugin-1)
* [`crawl-companies plugins:uninstall PLUGIN...`](#crawl-companies-pluginsuninstall-plugin-2)
* [`crawl-companies plugins update`](#crawl-companies-plugins-update)

## `crawl-companies hello PERSON`

Say hello

```
USAGE
  $ crawl-companies hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/jharrisonio/crawl-companies/blob/v0.0.0/dist/commands/hello/index.ts)_

## `crawl-companies hello world`

Say hello world

```
USAGE
  $ crawl-companies hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ crawl-companies hello world
  hello world! (./src/commands/hello/world.ts)
```

## `crawl-companies help [COMMAND]`

Display help for crawl-companies.

```
USAGE
  $ crawl-companies help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for crawl-companies.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.14/src/commands/help.ts)_

## `crawl-companies plugins`

List installed plugins.

```
USAGE
  $ crawl-companies plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ crawl-companies plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.1.1/src/commands/plugins/index.ts)_

## `crawl-companies plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ crawl-companies plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ crawl-companies plugins add

EXAMPLES
  $ crawl-companies plugins:install myplugin 

  $ crawl-companies plugins:install https://github.com/someuser/someplugin

  $ crawl-companies plugins:install someuser/someplugin
```

## `crawl-companies plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ crawl-companies plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ crawl-companies plugins:inspect myplugin
```

## `crawl-companies plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ crawl-companies plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ crawl-companies plugins add

EXAMPLES
  $ crawl-companies plugins:install myplugin 

  $ crawl-companies plugins:install https://github.com/someuser/someplugin

  $ crawl-companies plugins:install someuser/someplugin
```

## `crawl-companies plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ crawl-companies plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.

EXAMPLES
  $ crawl-companies plugins:link myplugin
```

## `crawl-companies plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ crawl-companies plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ crawl-companies plugins unlink
  $ crawl-companies plugins remove
```

## `crawl-companies plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ crawl-companies plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ crawl-companies plugins unlink
  $ crawl-companies plugins remove
```

## `crawl-companies plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ crawl-companies plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ crawl-companies plugins unlink
  $ crawl-companies plugins remove
```

## `crawl-companies plugins update`

Update installed plugins.

```
USAGE
  $ crawl-companies plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
