# ios_video-player
A simple video player app for iOS that plays a local video file using the AVKit and AVFoundation frameworks.

### Description

This app demonstrates how to create a video player for iOS using Swift. The code provided plays a local video file named "test.mp4" using the AVPlayer and AVPlayerViewController classes.

### Requirements

- Xcode 13.0 or later
- iOS 15.0 or later
- Test video file named "test.mp4"

### Usage

1. Clone or download this repository.
2. Open the project in Xcode.
3. Add a video file named "test.mp4" to the project. Make sure it is added to the "Copy Bundle Resources" build phase.
4. Run the app on a simulator or a physical device.

### Code Overview

`ViewController.swift` is the main view controller for the app, and it contains the following methods:

- `viewDidLoad()`: Called when the view controller's view has been loaded into memory. It is a good place to put any additional setup after loading the view.
- `viewDidAppear(_ animated: Bool)`: Called when the view controller's view is about to be added to a view hierarchy and appear on the screen. In this method, the `playVideo()` function is called.
- `playVideo()`: This function is responsible for playing the video file. It first checks if the "test.mp4" file is available in the app bundle. If the file is found, it initializes an AVPlayer object with the video URL and creates an instance of AVPlayerViewController. The AVPlayer object is then assigned to the player property of the AVPlayerViewController. The player view controller is presented modally, and the video starts playing when the presentation is complete.

### Troubleshooting

If the video does not play, make sure:

- The "test.mp4" file is included in the project and added to the "Copy Bundle Resources" build phase.
- The video file is named correctly and has the ".mp4" extension.
- The device or simulator you are running the app on supports the video codec of the "test.mp4" file.
