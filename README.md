Getting started on a new app just takes too damn long, though. Most apps need the same basic building blocks and developer infrastructure, and we are bored of reinventing the wheel time and time again.

This Starter Kit reflects the best practices of React Native development we have discovered while building real-world applications for our customers. It is opinionated about tooling, patterns and development practices. It might not be a one-size-fits-all solution for everyone, but feel free to customize it for your needs, or just take inspiration from it.


### Testing Setup

* [Mocha](https://mochajs.org/) for unit testing application code
* [Enzyme](https://github.com/airbnb/enzyme) and fully mocked React Native for unit testing UI components
* [Istanbul](https://github.com/gotwarlost/istanbul) code coverage
* Utilities for end-to-end integration testing Redux state, including side effects and asynchronous actions

### Development & Deployment Infrastructure

* [Auth0](https://auth0.com/) for ready-to-use login and signup screens, user authentication and identity management
* [Bitrise.io](https://www.bitrise.io) configurations for Continuous Integration and beta app distribution
* :warning: [Google Tag Manager](https://www.google.com/analytics/tag-manager/) analytics
* :star: [Microsoft Code Push](http://microsoft.github.io/code-push) for Continuous Deployment and instant app updates


### Roadmap

* **TODO** Crash reporting
* **TODO** Android and iOS UI Testing with Calaba.sh?
* **TODO** Feature flags?

## Getting started

To build your own app on top of the Starter Kit, fork or mirror this repository. For serious use we recommend [mirroring using these instructions](https://help.github.com/articles/duplicating-a-repository/), since you can't make a fork of a public repository private on GitHub. To contribute to Starter Kit development or just playing around, forking is the way to go.

First, give your application a name by running `./support/rename.sh YourAppName`.

Once you have the code downloaded, follow the **[Setup guide](docs/SETUP.md)** to get started.

## Development workflow

After you have set up the project using above instructions, you can use your favorite IDE or text editor to write code, and run the application from the command line. Turn on React Native hot module reloading in the app developer menu to update your application as you code.

To learn how to structure your application and use the Redux application architecture, read the **[Architecture guide](docs/ARCHITECTURE.md)** for more details.

##### Start the application in iOS simulator
```
$ react-native run-ios
```

##### Start the application in Android simulator
(If using the stock emulator, the emulator must be running)
```
$ react-native run-android
```

##### Run unit tests
```
$ npm test
```

##### Run tests every time code changes
```
$ npm run test:watch
```

##### Generate code coverage report
```
$ npm run coverage
```

Read the **[Testing guide](docs/TESTING.md)** for more information about writing tests.

## Deployment

Read the **[Deployment guide](docs/DEPLOYMENT.md)** to learn how to deploy the application to test devices, app stores, and how to use Code Push to push updates to your users immediately.

