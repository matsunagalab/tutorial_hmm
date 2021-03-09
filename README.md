# Hands-on tutorial on Data-assimilation with Markov state model and hidden Markov modeling

This repository is a set of Jupyter notebooks to help researchers already familiar with MD simulations lean how to integrate MD and experimental data with Markov state models (MSM) and hidden Markov modeling (HMM). 

## Getting started 

This is a hands-on tutorial and uses Jupyter notebook for illustrating live codes for computing MSM and HMM. So, you need to install Jupyter in your machine. In the case of MacOS, you can install it from python's package system:

```
$ pip3 install jupyterlab

# If the above didn't wok, some options may be required, such as
$ pip3 install jupyterlab --user

# Or superuser priviledges may be required
$ sudo pip3 install jupyterlab
```

Also, we use our in-house Julia package [MDToolbox.jl](https://github.com/matsunagalab/MDToolbox.jl) for using functions related to MSM and HMM. You need to download and install Julia from the [Julia website](https://julialang.org), or in the case MacOS, you can install via Homebrew:

```
$ brew install julia
```

After installing Julia, required packages can be installed as follows,

```
$ julia -e 'using Pkg; Pkg.add(["PyPlot", "JLD2", "IJulia"])'
$ julia -e 'using Pkg; Pkg.add(Pkg.PackageSpec(url="https://github.com/matsunagalab/MDToolbox.jl.git", rev="master"))'
$ julia -e 'using IJulia'

# If you already install an older version of MDToolbox, please update it by
$ julia -e 'using Pkg; Pkg.update("MDToolbox")'
```

Finally, let's download this repository from GitHub:

```
$ git clone https://github.com/matsunagalab/hmm_tutorials.git
$ cd hmm_tutorials/

# Or if you already downloaded older versions of the tutorial files, please update them by
$ cd hmm_tutorials/
$ git fetch origin main
$ git reset --hard origin/main
```

You are all set now. Let's start the tutorial by starting Jupyter Lab:

```
$ jupyter-lab
```

## Tutorial notebooks

* [Slides](https://github.com/matsunagalab/hmm_tutorials/blob/main/slides.pdf)
* 00 - [Preliminaries - Introduction to Julia and MDToolbox.jl](https://github.com/matsunagalab/hmm_tutorials/blob/main/00_Preliminaries.ipynb)
* 01 - [Markov State Model basics](https://github.com/matsunagalab/hmm_tutorials/blob/main/01_Markov_State_Model.ipynb)
* 02 - [Hidden Markov Model basics](https://github.com/matsunagalab/hmm_tutorials/blob/main/02_Hidden_Markov_Model.ipynb)
* 03 - [Data assimilation via MSM and HMM](https://github.com/matsunagalab/hmm_tutorials/blob/main/03_Data_Assimilation.ipynb)

## References

* Matsunaga and Sugita, JCP 2018
* Matsunaga and Sugita, eLife 2018
* Matsunaga and Sugita, Curr. Opin. Struct. Biol. 2020

