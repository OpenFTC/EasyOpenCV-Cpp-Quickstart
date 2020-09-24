# EasyOpenCV-Cpp-Quickstart

An example FTC Robot Controller project for running C++ OpenCV code through EasyOpenCV

# Version information

Currently based on FTC Robot Controller SDK v6.0

# Setup instructions

1. Ensure that you have version `21.0.6113669` of the side-by-side Android NDK installed
2. Fork this repo and clone your fork into a parent directory of your choice
3. Also clone [OpenCV-Repackaged](https://github.com/OpenFTC/OpenCV-Repackaged) **into the same parent directory** as you cloned this project. This is necessary because the build scripts in this project reference files that are in OpenCV-Repackaged.

    > Please note that if OpenCV-Repackaged ever upgrades to a newer version of the OpenCV library itself (it is currently on its 3rd release, but thus far all releases have been based on OpenCV 4.1.0), you will need to take care that the version of OpenCV-Repackaged you have checked out matches with the version of OpenCV-Repackaged used by the version of EasyOpenCV that you are using.

    Alternatively, you may copy the native headers and native library (for linking) into the project and edit the `Teamcode/CMakeLists.txt` build script accordingly.

4. Take a look at the `NativePipeline.java`, `NativePipelineExample.java`, and `native_pipeline.cpp` files in the TeamCode module. Build the project and deploy to your Android device, you're ready to go!
