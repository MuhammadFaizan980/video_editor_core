## 0.1.8
- **FIX**(android): Fixed crash during video export when applying overlay effects. The issue was caused by using `ImmutableList.of(bitmapOverlay)` instead of a Kotlin-compatible list. This has been resolved by using `listOf(bitmapOverlay)` instead.
- **CHORE**(android): Updated `media3` dependencies to the latest stable versions for better compatibility and stability.

## 0.1.7
- **FIX**(iOS, macOS): Resolved a crash that occurred when setting playback speed below 1x. This resolves issue [#29](https://github.com/hm21/pro_video_editor/issues/29).

## 0.1.6
- **FIX**(iOS, macOS): Fixed rotation transforms not properly swapping render dimensions for 90°/270° rotations, resolving squeezed video output with black bars.

## 0.1.5
- **FIX**(window, linux, iOS, macOS): Correct bitrate extraction from metadata. 
- **FIX**(android): Remove unsupported WebM output format; Android only supports MP4 generation. 
- **TEST**: Add integration tests for all core functionalities.

## 0.1.4
- **FIX**(iOS, macOS): Fixed AVFoundation -11841 "Operation Stopped" errors when exporting videos selected via image_picker package
- **FIX**(iOS, macOS): Fixed video rotation metadata not being properly handled, causing incorrect orientation in exported videos
- **FIX**(iOS, macOS): Fixed random video loading failures from image_picker package due to complex transform metadata
- **FIX**(iOS, macOS): Enhanced video composition pipeline to properly process iPhone camera orientation transforms

## 0.1.3
- **FIX**(iOS, macOS): Resolved multiple issue where, in some Swift versions, a trailing comma in the constructor caused an error.

## 0.1.2
- **FIX**(iOS, macOS): Resolved an issue where, in some Swift versions, a trailing comma in the constructor caused an error.

## 0.1.1
- **DOCS**: Updated README with new examples and images.

## 0.1.0* 
- **FEAT**(iOS): Added render functions for iOS.
- **FEAT**(macOS): Added render functions for macOS.

## 0.0.14
- **FIX**: Resolve various crop and rotation issues.
- **REFACTOR**(android): Improve code quality.
- **FEAT**(example): Add video-editor example.

## 0.0.13
- **FIX**(crop): Resolve issues that crop not working.

## 0.0.12
- **FIX**(layer): Fixed incorrect layer scaling caused by misinterpreted video dimensions.

## 0.0.11
- **FIX**(rotation): Resolve various issues when video is rotated.

## 0.0.10
- **FEAT**(native-code): Remove the ffmpeg package and start implementing native code.

## 0.0.9
- **REFACTOR**(encoding): Export encoding models for easier import from main package

## 0.0.8
- **FEAT**(audio): Add enable audio parameter

## 0.0.7
- **FEAT**(iOS, macOS): Add video generation support for macOS and iOS

## 0.0.6
- **FIX**(crop): Ensure crop dimensions are even to avoid libx264 errors

## 0.0.5
- **FEAT**: Add support for color 4x5 matrices

## 0.0.4
- **FEAT**: Add video parser functions for android

## 0.0.3
- **FIX**: Resolve thumbnail generation on web.

## 0.0.2
- **FEAT**: Add `getVideoInformation` and `createVideoThumbnails` for all platforms.

## 0.0.1

- **CHORE**: Initial release.
