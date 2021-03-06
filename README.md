[![Travis CI](https://api.travis-ci.org/rprieto/tldr-node-client.png)](https://travis-ci.org/rprieto/tldr-node-client) [![Dependency Status](https://david-dm.org/rprieto/tldr-node-client.png?theme=shields.io)](https://david-dm.org/rprieto/tldr-node-client) [![devDependency Status](https://david-dm.org/rprieto/tldr-node-client/dev-status.png?theme=shields.io)](https://david-dm.org/rprieto/tldr-node-client#info=devDependencies)

# tldr-node-client

A `Node.js` based command-line client for [tldr](https://github.com/rprieto/tldr).

![tldr screenshot](http://raw.github.com/rprieto/tldr-node-client/master/screenshot.png)

## Installing

[![NPM](https://nodei.co/npm/tldr.png)](https://www.npmjs.org/package/tldr)

```bash
$ npm install -g tldr
```

*Note: TLDR is still in early versions. We try to minimise breaking changes, but if you run into issues please try to download the latest package again.*

## Usage

To see tldr pages:

- `tldr <command>`
- `tldr --list` to show all available pages
- `tldr --random` to show a page at random

The client caches a copy of all pages locally, in `~/.tldr`.
There are more commands to control the local cache:

- `tldr --update` to download the latest "stable" pages
- `tldr --clear-cache` to delete the entire local cache

As a contributor, you might also need the following commands:

- `tldr --update --tag 1.2.3` to download a specific tag of the pages
- `tldr --update --branch somebranch` to download from a specific branch
- `tldr --update --github username:password` if you make more than 30 updates/hour for testing

## Configuration

You can configure the `tldr` client by adding a `.tldrrc` file in your HOME directory. This file has to be valid JSON.

```json
{
  "repository" : "rprieto/tldr",
  "colors": {
    "text": "green",
    "command-background": "black",
    "command-foreground": "red",
    "command-token": "white"
  }
}
```

## Contributing

Contribution are most welcome! Have a look [over here](https://github.com/rprieto/tldr-node-client/blob/master/CONTRIBUTING.md) for a few rough guidelines.
