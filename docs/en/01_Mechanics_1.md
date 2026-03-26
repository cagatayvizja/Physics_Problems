# Section 1: Mechanics I

\documentclass{article}
\usepackage[utf8]{inputenc}
\usepackage{amsmath}
\usepackage{amsfonts}
\usepackage{amssymb}
\usepackage{geometry}

\geometry{a4paper, margin=1in}

\begin{document}

\title{Mechanics I - Solutions Guide}
\author{Physics Presentation}
\date{\today}
\maketitle

\section*{1. Projectile Motion}
\textbf{Given:} $v_0 = 100 \text{ m/s}$, $\theta = 37^\circ$, $g = 9.8 \text{ m/s}^2$.

\subsection*{a) Differential Equations of Motion}
Assuming no air resistance:
\begin{itemize}
    \item Horizontal: $\frac{d^2x}{dt^2} = 0$
    \item Vertical: $\frac{d^2y}{dt^2} = -g$
\end{itemize}

\subsection*{b) Results}
\begin{itemize}
    \item \textbf{Time of Flight ($t_f$):} $t_f = \frac{2v_0 \sin\theta}{g} = \frac{2(100)(0.6)}{9.8} \approx \mathbf{12.24 \text{ s}}$
    \item \textbf{Maximum Height ($H$):} $H = \frac{(v_0 \sin\theta)^2}{2g} = \frac{(60)^2}{19.6} \approx \mathbf{183.67 \text{ m}}$
    \item \textbf{Range ($R$):} $R = \frac{v_0^2 \sin(2\theta)}{g} = \frac{100^2 \sin(74^\circ)}{9.8} \approx \mathbf{980.87 \text{ m}}$
\end{itemize}

\section*{2. Range Optimization}
To maximize $R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$, we find the derivative:
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta) = 0$$
$$\cos(2\theta) = 0 \implies 2\theta = 90^\circ \implies \mathbf{\theta = 45^\circ}$$

\section*{3. Path Intersection}
$A(t) = (2+t, 8-3t)$, $B(t) = (2t-1, 2t+2)$.
\begin{enumerate}
    \item Equate $x$: $2+t = 2t-1 \implies \mathbf{t=3 \text{ s}}$.
    \item Check $y$ at $t=3$: $y_A = -1$ and $y_B = 8$.
    \item \textbf{Result:} No collision because $y_A \neq y_B$ at the same time.
\end{enumerate}

\section*{4. Vector Calculus}
Given $\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$:
\begin{itemize}
    \item \textbf{Velocity:} $\vec{v}(t) = \frac{d\vec{r}}{dt} = \mathbf{6t\hat{i} + (5 - 16t)\hat{j}}$
    \item \textbf{Acceleration:} $\vec{a}(t) = \frac{d\vec{v}}{dt} = \mathbf{6\hat{i} - 16\hat{j}}$
\end{itemize}

\section*{5. Relative Velocity}
Let boat speed $v_b = 5$ and river $v_r = 2$. To go North:
$$\sin\theta = \frac{v_{river}}{v_{boat}} = \frac{2}{5} \implies \mathbf{\theta \approx 23.58^\circ \text{ upstream}}$$
Time to cross: $t = \frac{200}{\sqrt{5^2 - 2^2}} = \frac{200}{\sqrt{21}} \approx \mathbf{43.64 \text{ s}}$

\section*{6. Variable Velocity}
$v(t) = t^2 + 2t - 5$, $x(0)=4$.
\begin{itemize}
    \item \textbf{Position ($t=3$):} $x(3) = 4 + \int_0^3 (t^2+2t-5)dt = 4 + [9+9-15] = \mathbf{7 \text{ m}}$
    \item \textbf{Acceleration ($t=3$):} $a(t) = 2t+2 \implies a(3) = \mathbf{8 \text{ m/s}^2}$
\end{itemize}

\section*{7. Elimination of Time}
$x = 2t^2 \implies t = \sqrt{x/2}$.
Substitute into $y = 3t^3$: $\mathbf{y = 3(x/2)^{1.5}}$.
Acceleration $\vec{a}(t) = (4, 18t)$. It is \textbf{not constant} because it depends on $t$.

\section*{8. Circular Motion}
$R = 6378000 \text{ m}$, $T = 86400 \text{ s}$.
$$a_c = \frac{v^2}{R} = \frac{(2\pi R / T)^2}{R} = \frac{4\pi^2 R}{T^2} \approx \mathbf{0.0337 \text{ m/s}^2}$$

\section*{9. Momentum Comparison}
$p = mv$:
\begin{itemize}
    \item Fly: $0.002 \times 10 = \mathbf{0.02 \text{ kg}\cdot\text{m/s}}$
    \item Ball: $0.060 \times 1 = \mathbf{0.06 \text{ kg}\cdot\text{m/s}}$
\end{itemize}
The \textbf{tennis ball} has greater momentum.

\section*{10. Kinematics (Helix)}
$\vec{r}(t) = (a\cos\omega t, b\sin\omega t, bt)$.
The path is a \textbf{Helix}. Assuming $a=b$, the path length $s$ from $0$ to $t_0$ is:
$$s = \int_0^{t_0} \sqrt{(-a\omega\sin\omega t)^2 + (a\omega\cos\omega t)^2 + b^2} dt = \mathbf{t_0 \sqrt{a^2\omega^2 + b^2}}$$

\end{document}