# KMM Translator App

<img width="500" alt="kmm_project" src="https://github.com/user-attachments/assets/aa3ea153-8a0a-4558-ab6a-eee33927c972">

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Architecture](#architecture)
- [Technologies](#technologies)
- [Setup](#setup)
- [Testing](#testing)

## Description
This is a Kotlin Multiplatform (KMM) translator application designed to run on both Android and iOS platforms. The app leverages modern development practices such as Clean Architecture, Model-View-Intent (MVI) pattern, and platform-specific UI frameworks—Jetpack Compose for Android and SwiftUI for iOS.


## Features

- **Cross-Platform:** Runs seamlessly on both Android and iOS using Kotlin Multiplatform Mobile (KMM).
- **Clean Architecture:** The app follows the Clean Architecture principles, ensuring separation of concerns and testability.
- **Modern UI:** Built with Jetpack Compose for Android and SwiftUI for iOS.
- **MVI Pattern:** Implements the Model-View-Intent (MVI) pattern for a predictable, unidirectional data flow.
- **Offline Support:** Translations can be accessed offline once they have been fetched.
- **Multi-Language Support:** Translate between multiple languages with high accuracy.
- **Audio recognition:** Translate sentences by audio (permissions handle in each platform);

## Architecture

The app is built using Clean Architecture principles, separating the codebase into different layers:

- **Domain Layer:** Contains business logic and is platform-independent.
- **Data Layer:** Handles data operations, including API calls and database interactions. Uses interfaces to allow for dependency injection and easy testing.
- **Presentation Layer:** Manages the UI state using the MVI pattern. This layer interacts with the UI framework specific to each platform.

## Technologies

- **Kotlin Multiplatform (KMM):** Shared codebase between Android and iOS.
- **Jetpack Compose:** Declarative UI toolkit for Android.
- **SwiftUI:** Declarative UI framework for iOS.
- **Coroutines:** Handles asynchronous tasks.
- **Ktor:** Networking library used for making API calls.
- **SQLDelight:** Multi-platform SQL database library for storing translations.

## Setup

### Prerequisites

- **Android Studio** with KMM plugin installed.
- **Xcode** for building and testing the iOS version.

## Testing

The app includes both unit and UI tests for each platform.

Tests are written using:

- **JUnit** for unit testing in Kotlin.
- **Compose Test** for UI testing on Android.
- **XCTest** for unit and UI testing on iOS.
