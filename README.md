# Hands-on tutorial for Data-assimilation with Markov state model and hidden Markov modeling

This repository is a set of Jupyter notebooks to help researchers already familiar with MD simulations lean how to integrate MD and experimental data with Markov state models (MSM) and hidden Markov modeling (HMM). 

## Getting started 

This tutorial uses Jupyter notebook for illustrating real codes for computing MSM and HMM. So, you need to install the Jupyter plathome in your machine. In the case of MacOS, you can install it from python's package system:

```
$ pip3 install jupyterlab
```

Moreover, we use a julia package [MDToolbox.jl](https://github.com/matsunagalab/MDToolbox.jl) for calling specific functions related to MSM and HMM. You first need to install julia from the julia [website](https://julialang.org), or in the case MacOS, you can install via Homebrew:

```
$ brew install julia
```

After installing julia, MDToolbox.jl can be installed from julia REPL:

```
$ julia
julia> ]add https://github.com/ymatsunaga/MDToolbox.jl.git
julia> using MDToolbox
```

In order to use julia in Jupyter, IJulia package needs to be installed:

```
$ julia
julia> add IJulia
julia> using IJulia
```

Finally, let's download this repository from GitHub:

```
$ git clone https://github.com/matsunagalab/hmm_tutorials.git
$ cd hmm_tutorials/
```


## Tutorial notebooks

* 00 - [Preliminaries - Introduction to Julia and MDToolbox.jl](https://github.com/matsunagalab/hmm_tutorials/blob/main/00_Preliminaries.ipynb)
* 01 - [Markov State Model - Estimate transition probabilities from MD trajectories](https://github.com/matsunagalab/hmm_tutorials/blob/main/01_Markov_State_Model.ipynb)
* 02 - [Hidden Markov Model - Estimate transition probabilities from observation data](https://github.com/matsunagalab/hmm_tutorials/blob/main/02_Hidden_Markov_Model.ipynb)
* 03 - [Data assimilation via MSM - Combining MD with experimental data](https://github.com/matsunagalab/hmm_tutorials/blob/main/03_Data_Assimilation.ipynb)

## References

* Matsunaga and Sugita, JCP 2018
* Matsunaga and Sugita, eLife 2018

