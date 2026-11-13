# AF5-Pendulo-Robot
Actividad de simulación del comportamiento de un péndulo robot en python

Simulación en Python de un robot péndulo de 1 grado de libertad, a partir de la ecuación dinámica obtenida con el formalismo de Euler-Lagrange, en un tiempo total de 10 s.
Modelo

Con $x_1=q$ y $x_2=\dot q$:

$$\dot x_1 = x_2,\qquad \dot x_2 = \frac{1}{I_r}\left[\tau - m g l_c\sin x_1 - b x_2 - f_c\,\mathrm{sgn}(x_2)\right]$$

Parámetro	Valor
$I_r$	0.16 kg·m²
$m$	5 kg
$g$	9.81 m/s²
$l_c$	0.01 m
$b$	0.14 N·m·s/rad
$f_c$	0.45 N·m

Par de entrada: $\tau(t)=1.5\sin(t)$ N·m. Condiciones iniciales: $x_1(0)=0$, $x_2(0)=0$.

Cómo ejecutarlo
En Colab: abrir simulacion_pendulo_robot.ipynb desde Colab (Archivo → Abrir cuaderno → GitHub) y ejecutar todas las celdas.
Local: pip install -r requirements.txt y abrir la notebook con Jupyter.

Referencia
Cortés, F. R. (2020). Robótica: control de robots manipuladores. Marcombo.
