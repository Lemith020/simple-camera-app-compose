# Simple Camera App

A simple Android camera application built with Kotlin and Jetpack Compose for the Mobile Application Development assignment.

## Features

- Open the device camera
- Capture a photograph
- Display the captured photo inside the app
- Share the photo through the Android system share sheet (WhatsApp, Bluetooth, etc.)

## Tech Stack

- Kotlin
- Jetpack Compose (Material 3)
- ActivityResultContracts (TakePicture, RequestPermission)
- FileProvider
- Intent (ACTION_SEND) with Intent.createChooser
- Coil (image loading)
