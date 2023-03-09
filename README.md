# react-native-github-actions
CI/CD : React Native app integrated with Github Actions to deploy on playstore and App Store

1. Lint PR when raised against **dev**
2. Lint PR when raised against **stag** or **master** and close if linting fails
3. When PR merged in **master** or **stag**-

    - set android **release** group
    - bump version in package.json and react-native with a git tag
    - build and release on android and iOS