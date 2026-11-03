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

## Key Concepts

- **Camera permission:** declared in AndroidManifest.xml and requested at runtime before opening the camera.
- **Camera access:** the system camera is launched using the TakePicture contract, which saves the photo to a given Uri.
- **FileProvider:** creates a secure content:// Uri for the photo stored in the app cache.
- **Intents:** an ACTION_SEND intent carries the photo Uri to other apps.
- **Sharing interface:** Intent.createChooser opens the Android system share sheet.

- ## How It Works

1. Tap **Take Photo** and allow the camera permission.
2. The camera opens. Capture a photo and confirm it.
3. The captured photo is displayed in the app and the **Share** button appears.
4. Tap **Share** to open the Android share sheet and choose an app.

## Project Structure

```
app/src/main
├── AndroidManifest.xml
├── java/com/example/myapplication
│   └── MainActivity.kt
└── res/xml
    └── file_paths.xml
```
## Requirements

- Android Studio (latest stable version)
- Android device or emulator with camera support
- Minimum SDK as set in the project
