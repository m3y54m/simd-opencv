# Sobel Filter + SIMD + OpenCV

Using SIMD instructions in image processing using OpenCV

https://software.intel.com/sites/landingpage/IntrinsicsGuide/

https://en.wikipedia.org/wiki/Sobel_operator

## Build and Install OpenCV4

I've explained the build and installation steps in this gist: [Build OpenCV 4 in Ubuntu](https://gist.github.com/m3y54m/4f9b960e52f0da4e62e5a36f71d04fd7)

## Configure project

The recommended method for configuring OpenCV-based projects
is using CMake.

```console
sudo apt install cmake
```

The basic project configurations are written in
[`CMakeLists.txt`](https://github.com/opencv/opencv/blob/master/samples/cpp/example_cmake/CMakeLists.txt)
file which will be recognized by CMake tool. All source code of this project is in `src` directory.
In order to generate the Makefile and other files used to
build this project in a directory called `build` run these commands:

```console
cmake -S src -B build
```
## Build

```console
cmake --build build
```

Or first go to `build` directory with `cd build` command and execute this:

```console
cmake --build .
```

## Run

Supposed that you are in `build` directory:

```console
./sobel_simd_opencv
```
