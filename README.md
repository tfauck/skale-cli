# skale

[![Join the chat at https://gitter.im/skale-me/skale-cli](https://badges.gitter.im/skale-me/skale-cli.svg)](https://gitter.im/skale-me/skale-cli?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Build Status](https://travis-ci.org/skale-me/skale-cli.svg?branch=master)](https://travis-ci.org/skale-me/skale-cli)

Create, run and deploy distributed NodeJS applications

The skale command is the quickest and easiest way to create distributed
scalable applications based on
[skale-engine](https://www.npmjs.com/package/skale-engine) and then
to submit them either locally or on the cloud.

## Install

Assuming you have already installed [NodeJS](https://nodejs.org):

	$ npm install -g skale

## Getting started

To create an application called `my_app`, simply run

	$ skale create my_app

It will create a directory `my_app`, populate it with a template application
`my_app.js`, and install skale-engine dependency using [`npm`](https://npmjs.com).

You can then go to `my_app` and run your app using `skale run`:

	$ cd my_app
	$ skale run

To do something useful, modify your application by editing `my_app.js`,
then run again using `skale run`.

Under the hood, the `skale run` commands starts a skale-engine cluster on the
the localhost at the first invocation, then simply executes `my_app.js`. You
can check the status of the cluster using the `skale status` command, and stop
it using `skale stop`.

To go on further details, please refer to skale-engine documentation.
 
## Deploying an application

*Coming soon*

## Usage
```
Usage: skale [options] <command> [<args>]

Create, run, deploy clustered node applications

Commands:
  create <app>          Create a new application
  run [<args>...]       Run application
  deploy [<args>...]    Deploy application (coming soon)
  status                print status of local skale cluster
  stop                  Stop local skale cluster

Options:
  -h, --help            Show help
  -V, --version         Show version
```

## License

[Apache-2.0](LICENSE)
