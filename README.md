# react-native-github-actions
CI/CD : React Native app integrated with Github Actions to deploy on **AppCenter**[http://appcenter.ms/]

1. Lint PR when raised against **dev**
2. Lint PR when raised against **stag** or **master** and close if linting fails
3. When PR merged in **master** or **stag**-

    - set android **release** group
    - bump version in package.json and react-native with a git tag
    - build and release on android and iOS
    
    
## Getting Started

To run the app locally, you'll need to have Node.js and the React Native CLI installed. You can then clone the repository and install the dependencies using npm:

```$ git clone https://github.com/AnshulRaghav/react-native-github-actions.git```
```$ cd react-native-github-actions```
```$ npm install```
You can then run the app using the following command:

```$ npx react-native run-android```
This will launch the app in the Android emulator.

## Testing

To run the unit tests, use the following command:

```$ npm test```
To run the linting tests, use the following command:

```$ npm run lint```
These tests will run automatically as part of the CI pipeline when changes are pushed to the repository.

## CI/CD Pipeline

This app includes a CI/CD pipeline that is set up using GitHub Actions. The pipeline includes the following steps:

On each commit, the app is built and tested using the latest version of Node.js and React Native.
If the tests pass, the app is automatically deployed to a staging environment for further testing.
If the staging tests pass, the app is automatically packaged and deployed to the AppCenter.

## Contributing

If you'd like to contribute to this app, please fork the repository and create a pull request. Contributions are always welcome!

License

This app is licensed under the MIT License. See the LICENSE file for details.
