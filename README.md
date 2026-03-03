# Heun Centered In Time

### Discretization method


u-hat<sub>k</sub> - u<sub>k</sub><sup>n</sup> + (c/2)(u<sub>k+1</sub><sup>n</sup> - u<sub>k-1</sub><sup>n</sup>) = 0

u<sub>k</sub><sup>n+1</sup> - u<sub>k</sub><sup>n</sup> + (c/4)(u<sub>k+1</sub><sup>n</sup> - u<sub>k-1</sub><sup>n</sup> + u-hat<sub>k+1</sub> - u-hat<sub>k-1</sub>) = 0



## Stability




## Backward Error Analysis




## Theoretical Performance
Perforamnce at some level 
Our current implementation is CPU.

Psuedo code

```python

for t in time_steps:
    u_hat = udpate_u(...)
    u_next = full_step_solve(...)


`full_step_solve` O(k) 


```




## Parallel in time

