---
title: "Parallelizing PolyBench Kernels with MPI and OpenMP"
excerpt: "ETH course project (Design of Parallel and High-Performance Computing, team of four)."
collection: portfolio
---

Four PolyBench kernels (Gram-Schmidt, LU decomposition, covariance, correlation), each in MPI, OpenMP
and hybrid MPI+OpenMP C. Strong and weak scaling on ETH's Euler cluster up to 128 processes with
95% confidence intervals, PAPI FLOP counts per rank to check cyclic versus block load balancing, and a
cache-miss analysis of row- versus column-major layouts.
