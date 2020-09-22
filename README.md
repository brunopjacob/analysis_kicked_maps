# analysis_kicked_maps
Qualitative analysis of a periodically-kicked oscillator map using simulations in Julia

The model is given by the following map

\begin{align}
\theta_{\tau} & = \theta_0 + \tau + \frac{\sigma}{\lambda} \left[y_0 + A \sin(2 \pi \theta_0) (1 - e^{-\sigma \tau}) \right] \mod(1)\\
y_{\tau} & = e^{-\sigma \tau} \left[ y_0 + A \sin(2 \pi \theta_0) \right]\\
\end{align}

where $(\theta,y) \in \mathbb{S}^1 \times \mathbb{R}$, and $\sigma, \lambda, A, \tau$ are constants with $\sigma, \lambda, \tau > 0$.

For our parametric study, the parameters of interest are:

\begin{align}
\sigma &= \text{amount of shear}, \\
\lambda &= \text{rate of contraction to the limit cycle} \, \gamma = \{y=0\}, \\   
A &= \text{amplitude of kicks}, \\
\tau &= \text{time interval between kicks}.
\end{align}
