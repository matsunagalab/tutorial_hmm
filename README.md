# hmm_tutorials

This repository is a set of Jupyter notebooks to help researchers already familiar with MD simulations lean how to integrate MD and experimental data thourh Markov state modeling.

## Getting started 

This tutorial consits of several Jupyter notebook which are used in the Jupyter plathome. First, Jupyter needs to be installed in your machine. In the case of MacOS, you can install it from python's package system:

```
pip3 install jupyterlab
```

Moreover, we use a julia package [MDToolbox.jl](https://github.com/matsunagalab/MDToolbox.jl) for constructing a Marko state model and other stuff. So, you need to install julia from the julia [website](https://julialang.org), or in the case MacOS, you can install via Homebrew:

```
brew instal julia
```

After installing julia, MDToolbox.jl can be installed in julia REPL:

```
julia
julia> ]add https://github.com/ymatsunaga/MDToolbox.jl.git
julia> using MDToolbox
```

Moreover, in order to use julia in Jupyter, IJulia package needs to be installed:

```
julia
julia> add IJulia
julia> using IJulia
```

## Tutorial notebooks

* 01 - [Markov State Model]
* 02 - [Hidden Markov Model]
* 03 - [Data assimilation via MSM]


