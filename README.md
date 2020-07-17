# concaveman-cpp
C++ port of mapbox's JS [concaveman](https://github.com/mapbox/concaveman), with a Python wrapper

Please take a look at my [blog](https://adared.ch/concaveman-cpp-a-very-fast-2d-concave-hull-maybe-even-faster-with-c-and-python/) for a longer introduction :)

![Demo Screenshot](demo.png)


## Source changed:
Do not stdout in concaveman.cpp
Do not print points in concaveman.py

## Compile:
Go into concaveman-cpp/src/main/cpp
g++ -std=c++11 -shared -fPIC concaveman.cpp -o libconcaveman.so

Change path in concaveman-cpp/src/main/python/concaveman.py to the location (full path), where the libconcaveman.so resides.
