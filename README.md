# MPSCircuit.jl
A quick realization of MPS(Matrix Product State)-qubit circuit. 

# Supported types of MPS
- Cluster state
- Differentiable circuit constructed state

# Elements of the struct MPSC
Elements | Meanings
------------ | -------------
__circuit__|MPS circuit.
__cBlocks__|Array of all the MPS blocks in MPS circuit.
__cExtend__|The MPS circuit extended back to where it doesn't reuse any qubit.
__cEBlocks__|Array of all the MPS blocks in the Extended circuit.
__dGates__|Differentiable gates of the MPS circuit if applicable.
__nBit__|Number of lines(bits) of the MPS circuit. 
__nBlock__|Number of blocks in the MPS ciruict.

# Setup Guide
## Julia Environment
* [__Julia 1.1__](https://julialang.org)

## Installation
Please type `]` in Julia REPL to enter `Pkg` mode, then type:
```
pkg> add https://github.com/frankwswang/MPSCircuit.jl.git
``` 

## Dependent Packges
Please use the same method as above to install the packages below:

[__Yao__ (v0.3.2)](https://github.com/QuantumBFS/Yao.jl)
```
pkg> add Yao
``` 

[__QuAlgorithmZoo__](https://github.com/QuantumBFS/QuAlgorithmZoo.jl)
```
pkg> add https://github.com/QuantumBFS/QuAlgorithmZoo.jl.git
``` 


# Reference
* Variational Quantum Eigensolver with Fewer Qubits ([pdf](https://arxiv.org/pdf/1902.02663.pdf)), [arXiv:1902.02663](https://arxiv.org/abs/1902.02663), Jin-Guo Liu, Yihong Zhang, Yuan Wan and Lei Wang

# License
MPSCircuit.jl is released under Apache License 2.0.
