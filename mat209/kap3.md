# Koordinatentransformation

## Verschiebung eines kartesischen Koordinatensystems

Transformationsgleichungen zwischen alten Koordinaten (x,y) und neuen Koordinaten 

$
\left\{
\begin{array}
\tilde{x} = x - x_0 \\
\tilde{y} = y - y_0    
\end{array}
\right\} bzw.
\left\{
\begin{array}
xx = \tilde{x} + x_0 \\    
y = \tilde{y} + y_0
\end{array}
\right\}
$

## Drehung eines kartesischen Koordinatensystems

Transformationsgleichungen zwischen alten Koordinaten (x,y) und neuen Koordinaten (x,y) nach einer Drehung mit dem Winkel $\varphi$ um den Ursprung:

$
\tilde{x} = cos({\varphi})x + sin(\varphi)y \\
\tilde{y} = -sin({\varphi})x + cos(\varphi)y
$

## Transformation von kartesischen Koordinaten zu Polarkoordinaten

Die ***Polarkoordinaten*** (r,$\varphi$) eines Punktes (x,y) in der Ebene bestehen aus 

- den Abstand r des Punktes vom Koordinatenursprung und 
- dem Winkel $\varphi$ zwischen der positiven x-Achse und dem Ortsvektor zu dem Punkt.

Transformationsgleichungen von Polarkoordinaten zu kartesischen Koordinaten:

$r = \sqrt{x^2+y^2}, \varphi = 
\left\{ 
\begin{array}
    aarctan(x/y)   \quad für \quad x > 0 \\
    arctan(y/x) + \pi  \quad für \quad x < 0, \quad y \geq 0\\
    arctan(y/x) - \pi \quad für \quad x < 0, \quad y > 0 \\
    \pi/2 \quad für \quad x = 0, \quad y > 0\\
    -\pi/2 \quad für \quad x = 0, \quad y < 0 
\end{array}
\right\}
\in (-\pi, \pi]
$ 