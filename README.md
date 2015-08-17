
Android ScreenCapture Sample
===================================

This sample demonstrates how to use Media Projection API to capture device screen in real time and
show it on a SurfaceView.

Introduction
------------

Media Projection API lets you capture the current screen through Surface.

To start media projection, you need to get an instance of [MediaProjection][1]. For this, you have
to call startActivityForResult with an Intent from
[MediaProjectionManager.createScreenCaptureIntent()][2]. This shows a confirmation dialog to the
user. When user confirms it, you will get a result code and data in onActivityResult, so pass those
to [getMediaProjection][3].

Once you get a MediaProjection, use [createVirtualDisplay][4] and bind it to a Surface.

[1]: https://developer.android.com/reference/android/media/projection/MediaProjection.html
[2]: https://developer.android.com/reference/android/media/projection/MediaProjectionManager.html#createScreenCaptureIntent()
[3]: https://developer.android.com/reference/android/media/projection/MediaProjectionManager.html#getMediaProjection(int, android.content.Intent)
[4]: https://developer.android.com/reference/android/media/projection/MediaProjection.html#createVirtualDisplay(java.lang.String, int, int, int, int, android.view.Surface, android.hardware.display.VirtualDisplay.Callback, android.os.Handler)

Pre-requisites
--------------

- Android SDK v23
- Android Build Tools v23.0.0
- Android Support Repository

Screenshots
-------------

<img src="screenshots/main.png" height="400" alt="Screenshot"/> 

Getting Started
---------------

This sample uses the Gradle build system. To build this project, use the
"gradlew build" command or use "Import Project" in Android Studio.

Support
-------

- Google+ Community: https://plus.google.com/communities/105153134372062985968
- Stack Overflow: http://stackoverflow.com/questions/tagged/android

If you've found an error in this sample, please file an issue:
https://github.com/googlesamples/android-ScreenCapture

Patches are encouraged, and may be submitted by forking this project and
submitting a pull request through GitHub. Please see CONTRIBUTING.md for more details.

License
-------

Copyright 2014 The Android Open Source Project, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.
