# GoPhysics - Work in Progress

Go wrapper for the [Bullet Physics SDK](http://bulletphysics.org/wordpress/)

## Purpose
This wrapper aims to wrap the C++ classes of the Bullet physics library using SWIG, implementing unit and integration tests.


## Features
As far as is possible classes, functions, constants and enums will retain their names from the library.

## Limitations of Go
Some types from Bullet can not be wrapped in-place, requiring renaming and SWIG templating. These items include objects such as arrays and vectors that are used throughout Bullet. Other limitations include the allocating and accessing of memory, as these features of Bullet will be hidden where possible from the consumer of the library.

## Disclaimer
The project is currently intended as a learning experience for the author. As such it will take some time to implement. The reason Bullet is chosen as the target is the authors experience with Bullet and wrapping it for Python and C#.
