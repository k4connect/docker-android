## Android Docker Image for React Native (Experimental)

## Motivation
Provide Android SDK tools and Node.js for executing React Native builds

## Docker Hub Image
https://hub.docker.com/r/k4connect/react-native-android/

## Usage

**N.B. Need to ensure USB devices are accessible if using a physical Android device with which to develop. Currently, 

### Tested on Ubuntu (may work on macOS)
```
docker run -it --privileged -v /dev/bus/usb:/dev/bus/usb -v $(pwd):/workenv -w /workenv k4connect/react-native-android <YOUR_COMMAND_GOES_HERE>
```

### Original Source

This is a fork of an implementation of https://github.com/react-native-community/discussions-and-proposals/blob/master/proposals/0005-Official-Docker.md.

see https://hub.docker.com/r/reactnativecommunity/react-native-android/

Name may change later, see https://github.com/react-native-community/docker-android/issues/7.

Original version is split from react-native repo, see https://github.com/facebook/react-native/blob/988366a4179d87d667e5d9396efdfba4cbbe0b2e/ContainerShip/Dockerfile.android-base.

#### Showcase
https://github.com/react-native-community/ci-sample
