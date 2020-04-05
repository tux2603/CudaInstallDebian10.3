# Installing CUDA on Debian 10.3

I haven't figured out a way to get cuda installed yet. Right now, I'm going through the different installation options on the [nvidia site](https://developer.nvidia.com/cuda-downloads). It may or may not be necessary to build from source. 

## Lessons leaned

1. The local deb install for ubuntu 18.04 does not work well. The missing dependencies can be found [here](http://archive.ubuntu.com/ubuntu/pool/main/x/x-kit/python3-xkit_0.5.0ubuntu2_all.deb) and [here](https://launchpadlibrarian.net/424706799/screen-resolution-extra_0.18_all.deb) though.

## Instructions

I still haven't gotten CUDA working, but I am currently trying this method:

1. Download the local runfile for ubuntu 18.04 from the [nvidia site](https://developer.nvidia.com/cuda-downloads?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu&target_version=1804&target_type=runfilelocal)

