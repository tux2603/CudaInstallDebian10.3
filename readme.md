# Installing CUDA on Debian 10.3

I haven't figured out a way to get cuda installed yet. Right now, I'm going through the different installation options on the [nvidia site](https://developer.nvidia.com/cuda-downloads). It may or may not be necessary to build from source. 

## Lessons leaned

1. The local deb install for ubuntu 18.04 does not work well. The missing dependencies can be found [here](http://archive.ubuntu.com/ubuntu/pool/main/x/x-kit/python3-xkit_0.5.0ubuntu2_all.deb) and [here](https://launchpadlibrarian.net/424706799/screen-resolution-extra_0.18_all.deb) though.

## Instructions

As of Cuda 10.2.89 440.33.01, you can simply download the local runfile for ubuntu 18.04 and install. Newer versions of cuda have not been tested. Most recent kernel tested is 5.5.0

