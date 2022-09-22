# Stable Diffusion meets docker.

## Features

* Compatable with AMD cards, such as the RX580 and 5500XT
* Compatable on windows and linux, access to the container can be via command line or WebUI




### Developer notes
The docker container will be a base image of Arch linux, with the ROCM kernel installed. THe stable diffusion network will subsiquently be downloaded and configured on the startup of the container via a setup script.
The python tools required by Stable Diffusion will be auto installed by default, but needs to be overrided witht he ROCM version so they work.

So far the ROCM-Pytorch docker container works. But I and Kaz are still in the process of making the dedicated linux container.




