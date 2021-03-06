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
$ npm install -g airtable-automations
$ aira COMMAND
running command...
$ aira (--version)
airtable-automations/0.0.0 linux-x64 node-v17.3.0
$ aira --help [COMMAND]
USAGE
  $ aira COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`aira hello PERSON`](#aira-hello-person)
* [`aira hello world`](#aira-hello-world)
* [`aira help [COMMAND]`](#aira-help-command)
* [`aira plugins`](#aira-plugins)
* [`aira plugins:inspect PLUGIN...`](#aira-pluginsinspect-plugin)
* [`aira plugins:install PLUGIN...`](#aira-pluginsinstall-plugin)
* [`aira plugins:link PLUGIN`](#aira-pluginslink-plugin)
* [`aira plugins:uninstall PLUGIN...`](#aira-pluginsuninstall-plugin)
* [`aira plugins update`](#aira-plugins-update)

## `aira hello PERSON`

Say hello

```
USAGE
  $ aira hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Whom is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/dileep-kishore/airtable-automations/blob/v0.0.0/dist/commands/hello/index.ts)_

## `aira hello world`

Say hello world

```
USAGE
  $ aira hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ oex hello world
  hello world! (./src/commands/hello/world.ts)
```

## `aira help [COMMAND]`

Display help for aira.

```
USAGE
  $ aira help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for aira.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.10/src/commands/help.ts)_

## `aira plugins`

List installed plugins.

```
USAGE
  $ aira plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ aira plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.0.11/src/commands/plugins/index.ts)_

## `aira plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ aira plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ aira plugins:inspect myplugin
```

## `aira plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ aira plugins:install PLUGIN...

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
  $ aira plugins add

EXAMPLES
  $ aira plugins:install myplugin 

  $ aira plugins:install https://github.com/someuser/someplugin

  $ aira plugins:install someuser/someplugin
```

## `aira plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ aira plugins:link PLUGIN

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
  $ aira plugins:link myplugin
```

## `aira plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ aira plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ aira plugins unlink
  $ aira plugins remove
```

## `aira plugins update`

Update installed plugins.

```
USAGE
  $ aira plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
