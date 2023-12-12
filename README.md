# UPINN for Burger's equation
Universal Physics Informed Neural Network [(UPINN)](https://proceedings.mlr.press/v202/podina23a.html) applied on Burger's Equation:

$$
\frac{\partial  u}{\partial t} = -u \frac{\partial u}{\partial x} + \nu \frac{\partial^2 u}{\partial x^2}, \quad \nu=\frac{1}{100 \pi}, \quad u(x,0)=-\sin(\pi x)
$$

where the differential operator $-u \frac{\partial u}{\partial x}$ is assumed to be unknown and is approximated by a Neural Network $F(\vec{u};\theta_F)$.

<div style="display: flex;">
<figure>
  <img src="imgs/burgers_lbfgs.jpg" alt="Image 1" width="300">
  <img src="imgs/learned_u_slices.jpg" width="300">
  <figcaption>Approximated solution.</figcaption>
<figure>
</div>

<div style="display: flex;">
<figure>
  <img src="imgs/hidden_interaction.png" alt="Image 1" width="400">
  <figcaption>Unknown interaction: expected, learned and difference.</figcaption>
<figure>
</div>


