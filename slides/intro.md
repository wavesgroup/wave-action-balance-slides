<section>

### Wave heights from a global wave model (ecWAM)

![](assets/era5_Hs_2024-09-01.png)
</section>

<section>

### Peak wave period from a global wave model (ecWAM)

![](assets/era5_Tp_2024-09-01.png)
</section>


<section>

### Small-scale open ocean currents have large effects on wind wave heights

<img width="600" src="assets/Ardhuin_etal_2017_JGR_Fig01.png">

Fig. 1 from [Ardhuin et al. (2017)](https://doi.org/10.1002/2016JC012413)
</section>


<section>

## Wave action balance

The governing equation of ocean surface wave forecast models

$$
\frac{\partial N}{\partial t} + \nabla \cdot \left[\left(C_g + U\right) N \right] = \sum_{i=1}^{n} S_i
$$


* $\frac{\partial N}{\partial t}$: Wave action tendency
* $\nabla \cdot \left[(C_g + U) N \right]$: Wave action transport flux
* $\sum S_i$: Sources (e.g. wind) and sinks (wave breaking)

A simple yet historically tremendously successful equation used daily for surf forecasts, marine safety, shipping, coastal infrastructure etc.
</section>


<section>

## Where does wave action balance come from?

Whitham's (1965) variational approach:

$$
\delta \iint L\ dx\ dt = 0
$$

where $L$ is the instantaneous Lagrangian density (difference between the kinetic and the potential energy of the system):

$$
L = \int_{-h}^\eta \left[ \frac{\partial \phi}{\partial t} + \frac{1}{2} \left(\nabla \phi \right)^2 + gz \right] dz
$$
</section>


<section>

## Whitham's averaged variational principle

The phase-averaged Lagrangian density is:

$$
\mathcal{L} = \frac{1}{2\pi} \int_0^{2\pi} L\ d\psi
$$

Then, the averaged variational principle states:

$$
\delta \iint \mathcal{L} \ dx\ dt = 0
$$

And the averaged Lagrangian can be found to be:

$$
\mathcal{L} = \frac{1}{4} \left(1 - \frac{\omega^2}{gk} \right) ga^2 + \mathcal{O}(\varepsilon^4)
$$
</section>


<section>

## Bretherton & Garrett (1968)

In 1-D, deep water:

$$
\frac{\partial N}{\partial t} + \frac{\partial}{\partial x} \left[ \left(C_g + U\right) N \right] + \frac{\partial U}{\partial t} \frac{k}{\omega} N + \frac{\partial U}{\partial x} \frac{k}{\omega} C_g N = 0
$$

within small $\epsilon = \frac{1}{\omega U}\frac{\partial U}{\partial t}, \frac{1}{k U}\frac{\partial U}{\partial x}$

If $\epsilon \rightarrow 0$:

$$
\frac{\partial N}{\partial t} + \frac{\partial}{\partial x} \left[ \left(C_g + U\right) N \right] = 0
$$

This form (slowly and weakly varying currents) is assumed in all spectral wave models.

</section>


<section>

## Bretherton & Garrett (1968)

In 1-D, deep water, simplified

$$
\frac{\partial N}{\partial t} + C_g \frac{\partial N}{\partial x} + U \frac{\partial N}{\partial x} + N \frac{\partial U}{\partial x} + \frac{1}{2} N \frac{\partial u'}{\partial x} = 0
$$

within small $\epsilon = \frac{1}{k U}\frac{\partial U}{\partial x}$
</section>



<section>

## Governing equation, explained

$$
\frac{\partial N}{\partial t} + C_g \frac{\partial N}{\partial x} + U \frac{\partial N}{\partial x} + N \frac{\partial U}{\partial x} + \frac{N}{C_p} \frac{\partial U}{\partial t} + \frac{1}{2} N \frac{\partial u'}{\partial x} = 0
$$

* $\frac{\partial N}{\partial t}$: Wave action tendency
* $C_g \frac{\partial N}{\partial x}$: Wave propagation
* $U \frac{\partial N}{\partial x}$: Wave advection by mean currents
* $N \frac{\partial U}{\partial x}$: Wave strain by mean currents
* $\frac{1}{2} N \frac{\partial u'}{\partial x}$: Wave strain by subgrid-scale currents

What is the effect of unresolved currents on wave propagation?
</section>
