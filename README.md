# IO PagoPA Commons

This module provides code shared by the projects of the
[IO App](https://github.com/pagopa/io)
initiative.

## Contributing

In the following there are instructions to build the app in your computer for development purposes.

### Pre-requisites

We built a script for helping setting up the laptop, you can find it [here](https://github.com/pagopa/developer-laptop)

Otherwise, please follow the following steps:

#### Install NodeJS
To run the project you need to install a properly version of NodeJS.

On macOS and Linux we recommend the use of a virtual environment, such as nodenv for managing multiple versions of NodeJS.
The node version used in this project is stored in .node-version.

If you already have nodenv installed and configured on your system, the correct version node will be set when you access the app directory.

To install, follow the steps described below.

#### Install brew

If you do not have it already, install brew following the installation instructions in the [home page](https://brew.sh/).

#### Install nodenv

```
brew install nodenv
```

#### Install yarn

For the management of javascript dependencies we use Yarn.

Yarn is a node application. IF you have already installed in your system version of node compatible with yarn, you can install it as a global command with:

```
npm install -g yarn
```

### Install dependencies and build

Install the libraries used by the project and build it:

```
$ yarn install --frozen-lockfile
$ yarn build
```

### Run Tests

#### Run Unit Tests 

```
$ yarn test
```
#### Run Lint Check

```
$ yarn lint
```



### Releasing a version

Release has been automatized by using Azure Pipelines.

To release a new version please go to [io-pagopa-commons project on Azure](https://dev.azure.com/pagopa-io/io-pagopa-commons) and manually run _pagopa.io-pagopa-commons.deploy_ the pipeline.
Be aware to choose the right release version between major|minor|patch
