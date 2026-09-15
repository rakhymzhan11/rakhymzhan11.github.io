+++
title = "Code"
+++

Solvers behind my papers, released under the MIT licence. Everything is written from scratch; nothing depends on a pricing library. All repositories are at [github.com/rakhymzhan11](https://github.com/rakhymzhan11).

* [DSINC-AMERICAN-HESTON](https://github.com/rakhymzhan11/DSINC-AMERICAN-HESTON) (Python). Two independent pricers for American and European puts under the Heston model: a spectral damped-sinc integral-equation method with a piecewise-linear exercise boundary, and an MCS-ADI finite difference benchmark with policy iteration. Accompanies the paper with Leif Andersen and Andrey Itkin on American options and flexible forwards in time-dependent models.
* [DF-ADI](https://github.com/rakhymzhan11/DF-ADI) (MATLAB). Numerical results for *Diagonal Frog meets ADI: trading matrix exponentials for rational maps in the Fokker--Planck equation*, with Andrey Itkin. Each script is self-contained.
* [duopoly-resource-fd](https://github.com/rakhymzhan11/duopoly-resource-fd) (MATLAB). Monotone finite difference solvers with Howard policy iteration for the coupled HJB system of a two-firm stochastic resource game with risk-averse players and stochastic prices. Accompanies *The two faces of risk in the tragedy of the commons*, with Christian Ewald and Kevin Kamm.
