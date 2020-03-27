JHUGen
======
To install, run
$ lib/downloadcollier.sh
then
$ cd JHUGenerator/
$ make

then
$ ./JHUGen [arguments]

In case of error related to .dylib, run
$ install_name_tool -add_rpath ../lib/COLLIER  ./JHUGen
which may happen on the latest MacOS

