# Installing CUDA on Debian 10.3

1. Follow the instructions at [nvida'a site](https://developer.nvidia.com/cuda-downloads?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu&target_version=1804&target_type=deblocal) to get an installation file. The command `sudo apt install cuda` will fail due to unmet dependencies.

2. The dependency package that fails to install is `nividia-settings`, which has a dependencies `screen-resolution-extra` and `python3-xkit`, which aren't in the debian repository. They can be downloaded at the following locations:
..* [`python3-xkit`](http://archive.ubuntu.com/ubuntu/pool/main/x/x-kit/python3-xkit_0.5.0ubuntu2_all.deb)
..* [`screen-resolution-extra`](https://launchpadlibrarian.net/424706799/screen-resolution-extra_0.18_all.deb)

3. Once the .deb files for the dependencies are downloaded, install `python3-xkit` with the command `sudo dpkg -i python3-xkit_0.5.0ubuntu2_all.deb`

4. Then install `screen-resolution-extra` with the command `sudo dpkg -i screen-resolution-extra_0.18_all.deb`

5. Re-run the command `sudo apt install cuda`. this will pull down all of the necessary packages, but will fail because the required nvidia kernel module probably isn't loaded.

6. Reboot your computer to load the nvidia kernel module.
