# AR-ballGrabThrow
An Android AR app made in Unity 6 and AR Foundation. Grab a ball with your finger, flick to throw it, and watch it bounce off your real floor.

# AR Ball Throw

An Android augmented reality app built in Unity 6 (6000.0.85f2) with AR Foundation and ARCore. A ball appears in front of the camera. Touch it, drag it, and flick to throw it. It bounces off the real floor.

## How it works
- **BallGrabThrow** – raycasts from the camera to grab the ball on touch, follows the finger, measures swipe speed, and launches the ball on release. It respawns after 5 seconds.
- **FloorCollider** – uses AR Foundation plane detection to place an invisible floor at the lowest detected floor height.

## Requirements
- Unity 6000.0.85f2 with Android Build Support (OpenJDK, SDK and NDK)
- Android phone that supports ARCore (Android 7.0 / API 24 or higher)
- Built-In Render Pipeline, OpenGLES3 graphics API, IL2CPP, ARM64

## Build and run
1. Open the project in Unity.
2. File > Build Profiles > Android > Switch Platform.
3. Connect your phone with USB debugging on, then Build And Run.
4. Sweep the phone over the floor for 3–5 seconds, then grab and throw the ball.

## Install the APK
Download the APK from [Releases](../../releases) and allow "Install unknown apps" if Android asks.

## Notes
- Touch input only works on a device, not in the Unity Editor.
- On Unity 2022, change `rb.linearVelocity` to `rb.velocity`.

## Built with
Unity 6, AR Foundation, ARCore XR Plugin, C#
