# Scorpio

<h2 align='center'>Overview </h2>

---

The Scorpio MHD code with two fluid ambipolar diffusion solvers will be released in the near future.

Scorpio is a grid-based two-fulid hydrodynamic (HD) and magnetohydrodynamic (MHD) code, with ambipolar diffusion (AD), self-gravity (SG) and turbulence driving.The development of Scorpio is led by Dr. Hsiang Hsu Wang based on his experiencewith the MHD code Antares and inspired by our AD observation on NGC 6334 (Tanget al. 2018). Both Antares and NGC 6334 belong to the Scorpio constellation, thus the name of the code.

- Written in FORTRAN and MPI-parallelized.
- Based on Godunov-type shock-capturing finite volume method, the conservationparts are evolved in second-order of accuracy both in space and time, includingRiemann solvers (HLL, HLLC, HLLD) combined with a piecewise linear method(PLM) interpolation and Minimod limiter.
- The Poisson’s equation for self-gravity is solved using Fast Fourier Transformation(FFT) method.
- Turbulencing driving to perturb velocity field using FFT.
- The collision term of ambipolar diffusion is integrated using semi-implicit methodto overcome the stiffness.
- Time integration with the second-order Runge-Kutta method (RK2).
- Several featured test cases are presented to demonstrate the accuracy of Scorpio.

---

Read the [Scorpio Wiki](https://github.com/SFG-CUHK/scorpio-test-cases/wiki) for more details and test cases.
