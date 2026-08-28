# Astrophysical Hashed Oct Tree-based Smoothed Particle Hydrodynamics code 

## Description

This repository is the container (in the classical sense, not the Docker sense) for the codebase, in the past loosely referred to as "SNSPH", that contains the hashed oct tree in its two versions and the SPH codes built on top of those. 

## Repository structure

- **2hot**: the 'new' version of the hashed-oct-tree. Is GPU capable (up to inheriting applications to actually implement GPU kernels).

- **2hot-apps**: The main SPH applications from 'orig-tree16' that are partially ported to 2hot.

- **orig-tree16**: The original "SNSPH" code, includes the original hashed-oct-tree implementation. 

## Project status:

This entire codebase is currently in a state of flux. It is unlikely to build and run without considerable effort.

In the long term, the SPH applications are going to be ported to use 2hot, then to use GPUs. As part of this, unit tests and regression/integration tests are going to be developed to assert our expectations of code correctness and performance are met.

Until that effort is well underway, your best bet is to work with 'orig_tree16'.


## Contributing
tbd

## License and copyright


BSD 3-Clause License

Copyright (c) 2026, Los Alamos National Laboratory. O5196.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its
   contributors may be used to endorse or promote products derived from
   this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

