# Make: Magazine Article - Reinforcement Learning for Robotics

This repository accompanies the Make: Magazine article covering reinforcement learning (RL) for robotics.

> NOTE: all of the CLI commands are given for Debian-based Linux (e.g. Ubuntu). You will need to convert them if you wish to run this demo on another operating system (such as macOS or Windows).

## Train the Agent

Head to %%%LINK

In Google Colab, go to **Runtime > Change runtime type**. Under *Runtime version*, select **2026.07**. Click **Save**.l








## Installation

Make sure you have [Python 3.12+](https://www.python.org/) running on your system.

Download this repository: either click **Code > Download ZIP** or run the following:

```sh
git clone https://github.com/ShawnHymel/make-reinforcement-learning-for-robotics
```

Navigate into the directory:

```sh
cd make-reinforcement-learning-for-robotics
```

Create a Python virtual environment and install the requried Python packages:

```sh
python -m venv rl-env
source rl-env/bin/activate
pip install -r requirements.txt
```

> NOTE: we are installing the CPU-only version of PyTorch in this project. The simple balance bot agent can be trained in about an hour using most modern CPUs, which means you don't need an expensive GPU or need to download the CUDA version of PyTorch (saving you several GB of hard drive space).

## Train the Agent

Run JupyterLab:

```sh
jupyter-lab
```

Open a web browser and navigate to `localhost:8888`. The page will ask you for a token. Copy the hexadecimal token from the command line output (e.g. you should see a URL printed out ` http://localhost:8888/lab?token=<TOKEN>`. Copy `<TOKEN>`).

