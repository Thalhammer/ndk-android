# Docker android ndk image
Docker image with a minimal android user space.
This is used to run an application/library compiled
using the android ndk for x86/x86_64 on a regular
linux system.

## Building the image
Images get automatically built by docker hub. Each
api version is tracked by a separate branch which
gets pushed to a respective tag on dockerhub.

E.g. API Level 27 is pushed as "thalhammer/ndk-android:api-27".

NOTE: Currently the only supported api version is 27.

## Where does the "sys" folder come from ?
The binaries in the sys folder are pulled from the latest official avd
for each api level at the time of building. Note that
for obvious reasons there is no support for android specific features
like camera, OpenGL and so on.