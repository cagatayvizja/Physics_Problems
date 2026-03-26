# Section 1: Mechanics I - Solutions

## 1. Projectile Motion
Given: $v_0 = 100 \text{ m/s}$, $\theta = 37^\circ$. (Note: $\sin 37^\circ \approx 0.6, \cos 37^\circ \approx 0.8, g \approx 9.8 \text{ m/s}^2$)

* **Differential Equations:**
  $$\frac{d^2x}{dt^2} = 0, \quad \frac{d^2y}{dt^2} = -g$$
* **Time of Flight ($t_f$):**
  $$y(t) = v_0 \sin\theta t - \frac{1}{2}gt^2 = 0 \implies t_f = \frac{2v_0 \sin\theta}{g} = \frac{2(100)(0.6)}{9.8} \approx 12.24 \text{ s}$$
* **Maximum Height ($H$):**
  $$H = \frac{(v_0 \sin\theta)^2}{2g} = \frac{(60)^2}{19.6} \approx 183.67 \text{ m}$$
* **Range ($R$):**
  $$R = \frac{v_0^2 \sin(2\theta)}{g} = \frac{100^2 \sin(74^\circ)}{9.8} \approx 980.89 \text{ m}$$

---

## 2. Range Optimization
To find the maximum of $R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$, we take the derivative with respect to $\theta$:
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \cos(2\theta) \cdot 2 = 0$$
$$\cos(2\theta) = 0 \implies 2\theta = 90^\circ \implies \theta = 45^\circ$$

---

## 3. Path Intersection
Set $A(t) = B(s)$ (using different parameters for path intersection):
1. $2 + t = 2s - 1 \implies t = 2s - 3$
2. $8 - 3t = 2s + 2$

Substitute (1) into (2):
$$8 - 3(2s - 3) = 2s + 2 \implies 8 - 6s + 9 = 2s + 2 \implies 15 = 8s \implies s = 1.875$$
$$t = 2(1.875) - 3 = 0.75$$
**Intersection:** Since $t \neq s$, they cross the same point at different times. They do **not** collide.
**Intersection Point:** $A(0.75) = (2.75, 5.75)$.

---

## 4. Vector Calculus
$$\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$$
* **Velocity:** $\vec{v}(t) = \frac{d\vec{r}}{dt} = (6t)\hat{i} + (5 - 16t)\hat{j}$
* **Acceleration:** $\vec{a}(t) = \frac{d\vec{v}}{dt} = (6)\hat{i} + (-16)\hat{j}$

---

## 5. Relative Velocity
To go directly North, the horizontal component of boat velocity must cancel the river flow:
$$v_{boat} \sin\phi = v_{river} \implies 5 \sin\phi = 2 \implies \phi = \arcsin(0.4) \approx 23.58^\circ \text{ (West of North)}$$
* **Resultant Velocity:** $v_y = 5 \cos(23.58^\circ) \approx 4.58 \text{ m/s}$
* **Time:** $t = \frac{200}{4.58} \approx 43.67 \text{ s}$

---

## 6. Variable Velocity
$v(t) = t^2 + 2t - 5, \quad x(0) = 4$
* **Position:** $x(t) = \int v(t) dt = \frac{1}{3}t^3 + t^2 - 5t + C$. Since $x(0)=4, C=4$.
  $$x(3) = \frac{1}{3}(27) + 9 - 15 + 4 = 9 + 9 - 15 + 4 = 7$$
* **Acceleration:** $a(t) = \frac{dv}{dt} = 2t + 2 \implies a(3) = 2(3) + 2 = 8$

---

## 7. Elimination of Time
* **Eliminate $t$:** $t = \sqrt{x/2} \implies y = 3(x/2)^{3/2} = \frac{3}{2\sqrt{2}}x^{3/2}$
* **Vectors:**
  $$\vec{v}(t) = (4t, 9t^2), \quad |\vec{v}(t)| = \sqrt{16t^2 + 81t^4}$$
  $$\vec{a}(t) = (4, 18t), \quad |\vec{a}(t)| = \sqrt{16 + 324t^2}$$
* **Constant?** No, acceleration depends on $t$.

---

## 8. Circular Motion
$$a_c = \omega^2 R, \quad \omega = \frac{2\pi}{T}$$
$$T = 24 \times 3600 \text{ s}, \quad R = 6.378 \times 10^6 \text{ m}$$
$$a_c = \left(\frac{2\pi}{86400}\right)^2 \cdot 6.378 \times 10^6 \approx 0.0337 \text{ m/s}^2$$

---

## 9. Momentum Comparison ($p = mv$)
* **Fly:** $p = 0.002 \text{ kg} \cdot 10 \text{ m/s} = 0.02 \text{ kg}\cdot\text{m/s}$
* **Ball:** $p = 0.060 \text{ kg} \cdot 1 \text{ m/s} = 0.06 \text{ kg}\cdot\text{m/s}$
**The tennis ball has greater momentum.**

---

## 10. Kinematics (Helical Path)
**a) Trajectory:**
Projected on XY plane: $\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = \cos^2(\omega t) + \sin^2(\omega t) = 1$ (Elliptical Cylinder).
Since $z = bt$, it is an **Elliptical Helix**.

**b) Path Length ($s$):**
$$\vec{v}(t) = (-a\omega \sin\omega t, b\omega \cos\omega t, b)$$
$$|\vec{v}(t)| = \sqrt{a^2\omega^2 \sin^2\omega t + b^2\omega^2 \cos^2\omega t + b^2}$$
$$s = \int_0^{t_0} \sqrt{a^2\omega^2 \sin^2\omega t + b^2\omega^2 \cos^2\omega t + b^2} \, dt$$

**c) Special Case:** If $a=b$, it becomes a **Circular Helix**.