## Adversarial Training for self driving car

> Adversarial training for autonomous vehicle

Based on adversarial attack mentioned in [[ Paper ]](https://arxiv.org/abs/2103.09151)

The behaviour of end-to-end autonomous driving model can mititgate adversarial attack by adding few safety mechanisms..


### Quick Start

You may use [anaconda](https://www.continuum.io/downloads) or [miniconda](https://conda.io/miniconda.html). 

```python
$ git clone https://github.com/MJavaadAkhtar/Adversarial-training
$ cd adversarial-driving/model

$ # CPU
$ conda env create -f environment.yml
$ conda activate adversarial-driving

$ # GPU
$ conda env create -f environment_gpu.yml
$ conda activate adversarial-gpu-driving

$ python drive.py model.h5 
```

_note_: model.h5 is the newest trained model
This simulator was built for Udacity's Self-Driving Car Nanodegree, and it's available [here](https://github.com/udacity/self-driving-car-sim) (Download the zip file, extract it and run the executable file).

```
$ cd adversarial-driving/simulator/
$ ./Default\ Linux\ desktop\ Universal.x86_64
```

Version 1, 12/09/16

[Linux](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f0f7_simulator-linux/simulator-linux.zip)
[Mac](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f290_simulator-macos/simulator-macos.zip)
[Windows 32](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f4b6_simulator-windows-32/simulator-windows-32.zip)
[Windows 64](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f3a4_simulator-windows-64/simulator-windows-64.zip)


Your can use any web server, just serve all the content under **client/web**.

If you use windows, click on **client/client.exe**. It's a single executable that packages everything.

For Linux and Mac, or other Unix, the server can be built with:

```
$ cd adversarial-driving/client
$ go install github.com/gobuffalo/packr/v2@v2.8.3
$ go build
$ ./client
```

The web page is available at: http://localhost:3333/


