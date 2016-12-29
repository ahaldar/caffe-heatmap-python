# Installation

See http://caffe.berkeleyvision.org/installation.html for the latest
installation instructions.

Check the users group in case you need help:
https://groups.google.com/forum/#!forum/caffe-users

# Additional Notes

### For MatCaffe implememtation:
Caffe’s MATLAB interface works with versions 2015a, 2014a/b, 2013a/b, and 2012b.
CMake fails for MATLAB build
Build using Make after relevant changes to Makefile.config

`make all`
`make matcaffe`
`make test`
`make mattest`
`make runtest`

Creating symbolic links where necessary in bin/glnxa64 solves most "cannot find -l<nameOfTheLibrary>" issues:
https://github.com/BVLC/caffe/issues/3934

Edit initCaffe.m for appropriate gpu_id

### For PyCaffe implementation:
Run the following:
`make pycaffe`
`make runtest`

Edit initCaffe.py for appropriate gpu_id

Install modules that are imported for the project:
python3-scipy
python3-skimage

### For Ubuntu 16.04:
https://github.com/BVLC/caffe/wiki/Ubuntu-16.04-or-15.10-Installation-Guide
Creating symbolic links where necessary solves most "cannot find -l<nameOfTheLibrary>" issues:
https://github.com/BVLC/caffe/issues/4333
https://github.com/BVLC/caffe/issues/4045



