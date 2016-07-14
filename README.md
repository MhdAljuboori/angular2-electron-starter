# Angular2 and Electron Starter

Angular 2 and electron starter template, built using [Electrogram](https://github.com/onehungrymind/electrogram)

## Prerequisites
You will need to have [Git](https://git-scm.com/) and [Node.js (5.x and above) + NPM (3.x and above)](http://nodejs.org). We generally suggest installing [`NVM`](https://github.com/creationix/nvm) to manage Node versions. Once those are installed, you will need to install the `typings` NPM package globally. `Typings` handles the typescript definition files for our application.

## Getting started

First you will need to clone the repo; then you can install the necessary NPM packages and run the app.

```bash
# Clone the repo and enter it
git clone https://github.com/MhdAljuboori/angular2-electron-starter.git
cd angular2-electron-starter

# Install dependencies
npm i

# Install type definitions
typings install

# To build only
npm run build

# To build and watch for changes
npm run watch

# Start the Electron app
npm start # runs "electron src"
```

## Distributing the app
We've included an NPM script that will build a distrubtion version of the app for OSX. To use it, execute `npm run distribute`; this will create an OSX app that you can run from your Finder. For more info, check out https://github.com/electron-userland/electron-packager.

## The code
Here is a quick overview of the project structure:
```
Angular2ElectronStarter/
 ├──src/                       * contains the electron app script, html file, and all Angular code
 │   │
 │   ├──index.html             * parent HTML page where we include our built javascript files
 │   ├──main.js                * NodeJS script that bootstraps the Electron app
 │   │
 │   ├──app/                   * our Angular app has one "app" component, and this holds all the related code
 │   │   ├──boot.ts            * boot file
 │   │   ├──components         * components folder
 │   │       ├──app.ts         * app component functionality
 │   │
 │   └──assets/                * static assets are served here
 │       ├──css/               * global styles
 │       └──images/            * app logo and icon
 │
 ├──webpack.config.js          * configuration file that Webpack uses to build the app
 ├──tsconfig.json              * config that webpack uses for typescript
 ├──typings.json               * our typings manager
 └──package.json               * what npm uses to manage it's dependencies and scripts
 ```

## Author
A Sterter template built using [Electrogram](https://github.com/onehungrymind/electrogram) app.
