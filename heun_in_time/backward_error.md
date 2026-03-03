# Backward Error Analysis

In this section, we derive the backward error for the numerical scheme, taking into account the discretisation of both the **time** and **space** derivatives.

---

## Time Discretisation

The time derivative is approximated using a forward finite difference:


$u_t \approx \frac{u^{n+1} - u^{n}}{\Delta t}$


---

## Space Discretisation

The spatial derivative is approximated using a central finite difference:

\$u_x \approx \frac{u_{k+1} - u_{k-1}}{2\Delta x}$

---

## Backward Error Expression

For the advection equation

\$u_t + au_x = 0$

the combined time–space discretisation yields the following backward (modified‑equation) error:

\$u_t + au_x =
\frac{1}{48}(\Delta x)^2 u_{xxx}\left(c^2 - 8\right)
+
\mathcal{O}\left((\Delta x)^4,(\Delta t)^4\right)$

where

\$c = \frac{a\Delta t}{\Delta x}$

is the Courant number.

---
