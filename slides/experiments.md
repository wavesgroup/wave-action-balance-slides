<section>

## Numerical experiments

<div style="display: flex; justify-content: space-between;">
  
  <div style="flex: 1;">
    <ul>
      <li>Propagate a wave train in 1-d south to north, every 6 hours, for 24 hours, using the wave action balance equation (121 ensemble members each)</li>
      <li>Run using current fields at 150, 300, 600, 1200, 2400, 4800 m resolution</li>
      <li>Quantify terms contributions to the action tendency</li>
    </ul>
  </div>
  
  <div style="flex: 1;">
    <img src="assets/roms-150m-v-component-transect.png" width="300">
  </div>

</div>

$$
\frac{\partial N}{\partial t} + C_g \frac{\partial N}{\partial x} + U \frac{\partial N}{\partial x} + N \frac{\partial U}{\partial x} + \frac{1}{2} N \frac{\partial u'}{\partial x} = 0
$$

</section>


<section>

## Experiments summary

* **Experiment 1:** No currents, only wave propagation
$$
\frac{\partial N}{\partial t} + C_g \frac{\partial N}{\partial x} = 0
$$

* **Experiment 2**: Grid-resolved currents
$$
\frac{\partial N}{\partial t} + C_g \frac{\partial N}{\partial x} + U \frac{\partial N}{\partial x} + N \frac{\partial U}{\partial x} = 0
$$

* **Experiment 3**: Grid-resolved currents + subgrid-gradient strain
$$
\frac{\partial N}{\partial t} + C_g \frac{\partial N}{\partial x} + U \frac{\partial N}{\partial x} + N \frac{\partial U}{\partial x} + \frac{1}{2} N \frac{\partial u'}{\partial x} = 0
$$
</section>


<section>

### Experiment 1: No currents

<img src="assets/simulations/without-currents/surface_grid_L0150m_action1d_k1_t0000.png">
</section>


<section>

### Experiment 2: With currents, no subgrid strain, 150-m resolution

<img src="assets/simulations/without-strain/surface_grid_L0150m_action1d_k1_t0600.png">
</section>


<section>

### Experiment 2: With currents, no subgrid strain, 300-m resolution

<img src="assets/simulations/without-strain/surface_grid_L0300m_action1d_k1_t0600.png">
</section>


<section>

### Experiment 2: With currents, no subgrid strain, 600-m resolution

<img src="assets/simulations/without-strain/surface_grid_L0600m_action1d_k1_t0600.png">
</section>


<section>

### Experiment 2: With currents, no subgrid strain, 1200-m resolution

<img src="assets/simulations/without-strain/surface_grid_L1200m_action1d_k1_t0600.png">
</section>


<section>

### Experiment 2: With currents, no subgrid strain, 2400-m resolution

<img src="assets/simulations/without-strain/surface_grid_L2400m_action1d_k1_t0600.png">
</section>


<section>

### Experiment 2: With currents, no subgrid strain, 4800-m resolution

<img src="assets/simulations/without-strain/surface_grid_L4800m_action1d_k1_t0600.png">
</section>



<section>

### Experiment 3: With currents + subgrid strain, 300-m resolution

<img src="assets/simulations/with-strain/surface_grid_L0300m_action1d_k1_t0600.png">
</section>


<section>

### Experiment 3: With currents + subgrid strain, 600-m resolution

<img src="assets/simulations/with-strain/surface_grid_L0600m_action1d_k1_t0600.png">
</section>


<section>

### Experiment 3: With currents + subgrid strain, 1200-m resolution

<img src="assets/simulations/with-strain/surface_grid_L1200m_action1d_k1_t0600.png">
</section>


<section>

### Experiment 3: With currents + subgrid strain, 2400-m resolution

<img src="assets/simulations/with-strain/surface_grid_L2400m_action1d_k1_t0600.png">
</section>


<section>

### Experiment 3: With currents + subgrid strain, 4800-m resolution

<img src="assets/simulations/with-strain/surface_grid_L4800m_action1d_k1_t0600.png">
</section>