+++
template = "index.html"
title = "About"
+++

<img alt="Rakhymzhan Kazbek" id="avatar" src="/assets/images/photo.jpg" width="210" height="210" onerror="this.style.display='none'">

I am a post-doctoral researcher at [Umeå University](https://www.umu.se/en/) in Umeå, Sweden. My research currently applies stochastic differential game theory to financial economics in renewable and non-renewable resource management.

Previously I was a post-doctoral researcher at [Zayed University](https://www.zu.ac.ae/) in Abu Dhabi, UAE, working on parallel-in-time methods for large-scale problems in computational finance and derivative pricing, and an Assistant Professor in the Department of Computation and Data Science at [Astana IT University](https://astanait.edu.kz/).

I hold a PhD in Applied Mathematics, completed at [Nazarbayev University](https://nu.edu.kz/).

My research interests are focused on, but not limited to, quantitative finance, numerical analysis, scientific computing (HPC), operations research (combinatorial optimization for routing and graph network problems), stochastic optimal control in zero-sum and non-zero-sum settings (game theory), financial economics, and optimal stopping problems.

You can reach me at `rakhymzhan.kazbek@umu.se` or `rakhymzhankazbek@gmail.com`. I am also on [Google Scholar](https://scholar.google.com/citations?user=t0NgoNMAAAAJ), [LinkedIn](https://www.linkedin.com/in/rakhymzhan-kazbek-488b211a3/), and [GitHub](https://github.com/rakhymzhan11).

A CV is available on request.

## Research

I develop robust, high-performance numerical methods for pricing and hedging complex derivatives, with an emphasis on nonlinear problems: American-style contracts, optimal control, and models with market frictions.

* **Stochastic optimal control and games.** Optimal stopping and control in portfolio optimization, resource extraction, and strategic competition, leading to coupled HJB equations and quasi-variational inequalities.
* **PDEs in finance.** Finite difference and finite element (P1/P2) methods for linear and nonlinear pricing problems, including HJB equations, variational inequalities, and Volterra integral equations.
* **Stochastic methods and Monte Carlo.** Simulation-based pricing of vanilla and path-dependent derivatives across equities, commodities, rates, and FX, with variance reduction and robust Greeks.
* **Isogeometric analysis.** B-splines and NURBS for pricing PDEs, targeting non-smooth payoffs and stable sensitivities.
* **Parallel-in-time methods and HPC.** Multilevel Krylov, multigrid, and parareal algorithms for large-scale nonlinear problems, including American options as linear complementarity problems.
* **Combinatorial optimization.** Metaheuristics and deep reinforcement learning for constrained routing and graph network problems.

## Code

Solvers behind my papers, released under the MIT licence at [github.com/rakhymzhan11](https://github.com/rakhymzhan11). Everything is written from scratch; nothing depends on a pricing library.

* [DSINC-AMERICAN-HESTON](https://github.com/rakhymzhan11/DSINC-AMERICAN-HESTON) (Python). Two independent pricers for American and European puts under the Heston model: a spectral damped-sinc integral-equation method with a piecewise-linear exercise boundary, and an MCS-ADI finite difference benchmark with policy iteration. Accompanies the paper with Leif Andersen and Andrey Itkin on American options and flexible forwards.
* [DF-ADI](https://github.com/rakhymzhan11/DF-ADI) (MATLAB). Numerical results for *Diagonal Frog meets ADI: trading matrix exponentials for rational maps in the Fokker--Planck equation*, with Andrey Itkin.
* [duopoly-resource-fd](https://github.com/rakhymzhan11/duopoly-resource-fd) (MATLAB). Monotone finite difference solvers with Howard policy iteration for the coupled HJB system of a two-firm stochastic resource game with risk-averse players and stochastic prices. Accompanies *The two faces of risk in the tragedy of the commons*, with Christian Ewald and Kevin Kamm.
