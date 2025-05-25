# 📡 Applied Electromagnetics

This repository contains exercises, analytical formulations, and simulations related to applied electromagnetics. The tasks focus on solving boundary value problems and analyzing plane wave interactions with dielectric structures.

---

## ⚙️ Task 2 — Electrostatic Potential and Electric Field Visualization

Given the boundary conditions illustrated below:

![](image_1.png)

- $V = V_{0} = 10$ V at $y = 0$
- $V = V_{1} = V_{0} \sin\left( \frac{\pi x}{a} \right) = 10 \sin(\pi x)$ V at $y = b$
- $V = 0$ at $x = 0$ and $x = a$

With parameters:  
- $a = 1$ m  
- $b = 2$ m  

### Objective

> **(a)** Plot the electrostatic potential distribution $V(x, y)$.  
> **(b)** Plot the magnitude of the electric field $|E|$.

For two cases:  
- $n = 10$ (number of series terms)  
- $n = 50$ (number of series terms)

### Mathematical Formulation

The solution for the potential $V(x, y)$ inside the rectangular region is obtained via **Separation of Variables**, solving **Laplace’s Equation**:

$$
\nabla^2 V = 0
$$

The general solution is expressed as:

$$
V(x, y) = \sum_{n=1}^{\infty} A_n \sin\left( \frac{n\pi x}{a} \right) \sinh\left( \frac{n\pi y}{a} \right)
$$

The electric field is calculated from the negative gradient of the potential:

$$
\vec{E} = -\nabla V
$$

The magnitude of the electric field is:

$$
|E| = \sqrt{ \left( \frac{\partial V}{\partial x} \right)^2 + \left( \frac{\partial V}{\partial y} \right)^2 }
$$

---

## ⚙️ Task 3 — Wave Reflection on Dielectric Structures

### Problem 01 — Single Dielectric Slab (Both Sides Air)

A uniform plane wave at 10 GHz is normally incident on a dielectric plate of thickness $d$ and dielectric constant $\epsilon_r = 3.7$, bounded by air on both sides.

> **(a)** Calculate the thickness $d$ such that the input reflection coefficient is zero at 10 GHz. Repeat for 20 GHz.  
> **(b)** Plot the reflection coefficient magnitude versus frequency from 5 GHz to 30 GHz for a plate of $d = 0.9375$ cm, considering both 10 GHz and 20 GHz design frequencies.

---

### Problem 02 — Dielectric Slab with Semi-Infinite Medium

A uniform plane wave is incident normally on a dielectric slab whose thickness at $f_0 = 10$ GHz is $\lambda_{2_{0}}/4$, where $\lambda_{2_{0}}$ is the wavelength within the slab. The slab is bounded by air on the left and a semi-infinite medium with $\epsilon_{r_3} = 5.7$ on the right.

> **(a)** Find the intrinsic impedance $\eta_2$ and the dielectric constant $\epsilon_2$ of the slab such that the input reflection coefficient is zero at both 10 GHz and 20 GHz.  
> **(b)** Plot the reflection coefficient magnitude from 5 GHz to 30 GHz for the slab designed in (a).  
> **(c)** Using the ray-tracing model (Figure 5-11), compute the first and next two higher-order terms contributing to the reflection coefficient at 10 GHz and 20 GHz. Then, compute the total reflection coefficient using these three terms.

---

### Problem 03 — Binomial Matching with Two Dielectric Slabs

Two lossless dielectric plates, each with thickness $\lambda_0/4$ at $f_0 = 10$ GHz, are placed between air and a semi-infinite medium with $\epsilon_L = 6.7$. A binomial design is used with a fractional bandwidth of 0.375.

> **(a)** Compute the intrinsic impedances, dielectric constants, and physical thicknesses required for the plates to achieve zero reflection at 10 GHz and 20 GHz.  
> **(b)** Determine the maximum reflection coefficient and the standing wave ratio (SWR) within the bandwidth.  
> **(c)** Plot the reflection coefficient from 5 GHz to 30 GHz for this two-section binomial design. Compare it with the single-section design from Example 5-10.

---

### Problem 04 — Minimum Thickness Matching Plate

Design a dielectric plate (Figure 5-11a) with the smallest nonzero thickness such that the reflection coefficient at 1 GHz is zero. The plate is bounded by air on one side and a dielectric with $\epsilon_r = 16$ on the other.

> **(a)** Express the minimum thickness in terms of the wavelength within the plate.  
> **(b)** Calculate the thickness in centimeters at 1 GHz.  
> **(c)** Find the required dielectric constant of the plate.

Justify all answers assuming permeability $\mu = \mu_0$.

---

### Problem 05 — Ray Tracing vs Transmission Line Models

For the single-slab problem (Figure 5-11a), provide expressions for:

> **(a)** Exact transmission-line model.  
> **(b)** Exact ray-tracing model.  
> **(c)** Approximate ray-tracing model.

Using Example 5-9 ($d = 0.9375$ cm), plot the reflection coefficient magnitude for $5 \leq f \leq 15$ GHz:

> **(d)** Using the transmission-line model.  
> **(e)** Using the exact ray-tracing model.  
> **(f)** Using the approximate ray-tracing model.

Repeat for Example 5-10 ($d = \lambda_{2_0}/4$ at $f_0 = 10$ GHz):

> **(g)** Transmission-line model.  
> **(h)** Exact ray-tracing model.  
> **(i)** Approximate ray-tracing model.

---

### Problem 06 — Minimum Thickness Dielectric Slab

A dielectric slab of thickness $d$ is bounded by air on the left and a dielectric medium with $\epsilon_r = 16$ on the right (Figure 5-11a). Design the slab with the minimum nonzero thickness that eliminates the input reflection at 1 GHz.

> **(a)** Find the minimum thickness in terms of the wavelength inside the slab.  
> **(b)** Calculate the thickness in centimeters at 1 GHz.  
> **(c)** Determine the dielectric constant required for the slab.

Assume $\mu = \mu_0$ for all media.

---

## 📚 References

- **C. A. Balanis**, _Advanced Engineering Electromagnetics_, 2nd Edition, John Wiley & Sons, 2012.  
  🔍 Focus on **Chapter 5 — Reflection and Transmission**, particularly:  
  - Example 5-9  
  - Example 5-10  
  - Example 5-11  
  - Problem 5.41  
  - Problem 5.42  

- **Matthew N. O. Sadiku**, _Computational Electromagnetics with MATLAB_, 4th Edition, CRC Press, 2019.  
  🔍 Specifically **Example 2.1**, which covers the analytical solution of Laplace's equation in rectangular coordinates using the method of separation of variables.

---


## Lecture about Transmission Line

### References
> 

## Task 4

### References
> 
