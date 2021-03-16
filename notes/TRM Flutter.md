---
title: TRM Flutter
created: '2021-02-26T00:32:03.030Z'
modified: '2021-03-16T22:42:57.111Z'
---

# TRM Flutter

## Back-end App with Serverless, NodeJS and Apollo

### Pre-requisites
- Download and configure Android Studio -> https://developer.android.com/studio
- Download and configure Flutter -> https://flutter.dev/docs/get-started/install

## Getting Started

1) Clone the project
git clone project_path

2) Switch to resimax-stabilisation branch

3) Change channel for flutter `flutter channel flutter-1.22-candidate.8`

4) Change version in pubspec.yml `flutter: 1.22.0` 

5) Generate files
flutter pub get
flutter pub run build_runner build

6) Run the project (main_prod/main_dev, hpl/resimaxvip) 
`flutter run lib/main/hpl/main_dev.dart --flavor=hpl`

3) Run the build via one of commands (ios/apk, release/debug, hpl/resimaxvip)
flutter build ios -t lib/main/hpl/main_prod.dart --flavor=hpl --no-codesign
flutter build apk -t lib/main/hpl/main_prod.dart --flavor=hpl

## Updating files with codegeneration
After updating files that are used for codegeneration run:
flutter pub get
flutter packages pub run build_runner build --delete-conflicting-outputs
or with watch function
flutter packages pub run build_runner watch --delete-conflicting-outputs

## Custom Flutter Icons
For editing Trampoline Icons pack use file additional_data/config.json and service http://fluttericon.com/

## iOS GoogleService-Info.plist
- local build: file is copied via script Buid Phases -> Firebase Setup
- CI build: file is generated from the Environment variable

