<img align="right" src="media/HU.svg" alt="Hogeschool Utrecht">

# Adaptive Systems
Adaptive Systems - practica


Deze repository bevat code voor de practica van het vak *Adaptive Systems* van de Hogeschool Utrecht.

Neem bij vragen en opmerkingen contact op met de coördinator van het vak.

## Lunar lander

<img width="400" src="media/lunarlander_random.gif" alt="Lunar lander random"><br />


<img width="400" src="media/lunarlander_solved.gif" alt="Lunar lander solved">

### Prerequisites

Only install CUDA, cuDNN and tensorflow-gpu if you have a CUDA-supported NVidia GPU.

Tensorflow 2.10 is the last version with native Windows support. This version of
Tensorflow requires CUDA v11.8. This version of CUDA works well with cuDNN v8.*. 
Tensorflow 2.10 works well with Python 3.10.

* Install Microsoft Visual C++ Build Tools for Visual Studio
  * Visual Studio Installer
    * https://visualstudio.microsoft.com/downloads/
  * Add MSVC - VS 2022 C++ x64/x86 build tools (latest: v143)
  * Add Windows 10 SDK (latest: 10.0.20348.0)
* Install CUDA v11.8
  * https://developer.nvidia.com/cuda-11-8-0-download-archive
  * https://docs.nvidia.com/cuda/cuda-quick-start-guide/index.html
* Install cuDNN v8.9.7
  * https://developer.nvidia.com/cudnn-downloads
* Create conda environment: `conda create -n as python=3.10 pip`
* Activate the environment: `conda activate as`
* Install required packages:
  * `pip install tensorflow-gpu==2.10.0`
  * `pip install matplotlib`
  * `pip install swig`
  * `pip install gymnasium`
  * `pip install gymnasium[box2d]`
* Check installation:
  * `activate as`
  * `python` (should be version 3.10)
  * `import tensorflow as tf`
  * `tf.__version__` (should be version 2.10)
  * `tf.config.list_physical_devices('GPU')`
