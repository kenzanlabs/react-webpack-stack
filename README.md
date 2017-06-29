# react-seed

A seed / starter repo for React based UI applications

## Project Layout

An overview of important files and configurations for the applications

### Root Files ('dot' files)

Also know as 'dot' files, these are the build and build configuration files for the application

 * <i>bin/</i> - shell scripts for continuous integration and build environments
 * <i>.babelrc</i> - configuration file for Babel preproccessor
 * <i>.editorconfig</i> - configuration file for EditorConfig IDE plugin
 * <i>.eslintr</i>c - linting rules for spec and build files
 * <i>package.json</i> - NPM / Yarn dependency configuration file, for
 build related dependencies and defines all runnable scripts and commands
 * <i>webpack.config.common.js<i/> - webpack config for managing shared webpack configurations
 * <i>webpack.config.develop.js<i/> - webpack config for local development
 * <i>webpack.config.prod.js<i/> - webpack config for production builds

## Project Setup
Note: It is recommended that a Javascript based IDE is used, like Webstorm, as they have a lot of the code quality and syntax tooling supported as plugins, often times right out of the box.

### Steps

1. If you don't already have it, download and install NodeJS >=6.4.0 (comes with NPM).

1. This project favors Yarn, so make sure you have the latest by updating
it after installing Node by running

  ```
  $ npm install -g yarn@0.24.6
  ```

1. Now install the build and application dependencies by running

  ```
  $ yarn install
  ```

### Application Files

 Application code, including unit tests. Directories are intended to be
 kept as flat as possible with a B.O.F. (birds of a feather) organization.

```
react-seed
│
└───src
│   │
│   │
│   └───subfolder1
│       │   file111.txt
│       │   file112.txt
│       │   ...
│
└───folder2
    │   file021.txt
    │   file022.txt
```

## Tasks
This project uses Webpack as the build tool, executed via NPM scripts.
All available tasks are in the scripts section of package.json

### Development
This will start up a development server using
[webpack-dev-server](https://github.com/webpack/webpack-dev-server)
which watches for changes and 're-deploys' as needed.
```
$ yarn run develop
```

Webpack-dev-server will automatically open a browser window to ```localhost:9000```.

### Production
This is the production build task for the project. It is used prior to
deploying to an environment and builds a production version of the application.
This command cal also be used to serve a production build locally, it will automatically
open a browser window to ```localhost:9000```.

```
$ yarn run serve
```

## Project Setup
Note: It is recommended that a Javascript based IDE is used, like Webstorm, as they have a lot of the code quality and syntax tooling supported as plugins, often times right out of the box.

### Steps

1. If you don't already have it, download and install NodeJS >=6.4.0, which comes with npm.

1. This project favors Yarn, so make sure you have the latest by updating
it after installing Node by running

  ```
  $ npm install -g yarn@0.24.6
  ```

1. Now install the build and application dependencies by running

  ```
  $ yarn install
  ```

## Dependency Management
All dependencies added or removed from the project must be done so through yarn

### Add
```bash
# use --dev if it as devDependency
$ yarn add <package-name> [--dev]
```

### Remove
```
$ yarn remove <package-name>
```

### Upgrade
```
$ yarn upgrade <package-name>
```