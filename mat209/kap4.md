# Grenzwerte und Stetigkeit

## Grenzwerte für $x \rightarrow x_0$

Der ***(zweiseitige) Grenzwerte*** der Funktion $y=f(x)$ an der Stelle $x_0$ existiert und ist gleich $y_0$, wenn für alle $\epsilon > 0$ ein $\delta > 0$ existiert, so dass gilt:

$
|x-s_0| < \delta \quad \rightarrow \quad |f(x) - y_0| < \epsilon
$

$
\lim \limits_{x \to x_0} f(x) = y_0 \quad oder \quad
f(x)  \overset{x \rightarrow x_0}{\rightarrow} y_0 
$

Der ***linkseitige Grenzwert*** der Funktion $y = f(x)$ an der Stelle $x_0$ existiert und ist gleich $y_0$, wenn für alle $\epsilon > 0$ ein $\delta > 0$ existiert, so dass gilt:

$
0 < x_0 - x < \delta \Longrightarrow |f(x) - y_0| < \epsilon
$

Schreibweisen für den linksseitigen Grenzwert:

$
\lim \limits_{x \nearrow x_0} {f(x) = y_0} 
\quad oder \quad 
f(x) \overset{ x \nearrow x_0 }{\rightarrow} y_0
\quad oder \quad
\lim \limits_{x \rightarrow x_0^-} {f(x) = y_0}
$

Der ***rechtsseitige Grenzwert*** der Funktion $y = f(x)$ an der Stelle $x_0$ existiert und ist gleich $y_0$, wenn für alle $\epsilon > 0$ ein $\delta > 0$ existiert, so dass gilt:

$
0 < x_0 - x < \delta \Longrightarrow |f(x) - y_0| < \epsilon
$

Schreibweisen für den rechtsseitigen Grenzwert:

$
\lim \limits_{x \searrow x_0} {f(x) = y_0} 
\quad oder \quad 
f(x) \overset{ x \searrow x_0 }{\rightarrow} y_0
\quad oder \quad
\lim \limits_{x \rightarrow x_0^+} {f(x) = y_0}
$

$
\lim \limits_{x \to x_0} f(x) = y_0  \Longleftrightarrow \lim \limits_{x \nearrow x_0} {f(x) = \lim \limits_{x \searrow x_0} f(x) = y_0} 
$

Der ***Grenzwert*** der Funktion $y = f(x)$ an der Stelle $x_0$ ***existiert uneigentlich*** und ist gleich  $+\infty$, wenn für alle $K > 0$ ein $\delta > 0$ existiert, so dass gilt:

$
|x - x_0| < \delta \Rightarrow f(x) > K
$

Schreibweisen für den uneigentlichen Grenzwert $+\infty$:

$
\lim \limits_{x \to x_0} f(x) = +\infty \quad oder \quad f(x) \overset{ x \rightarrow x_0 }{\longrightarrow} +\infty
$

Der ***Grenzwert*** der Funktion $y = f(x)$ an der Stelle $x_0$ ***existiert uneigentlich*** und ist gleich  $-\infty$, wenn für alle $K < 0$ ein $\delta > 0$ existiert, so dass gilt:

$
|x - x_0| < \delta \Rightarrow f(x) < K
$

Schreibweisen für den uneigentlichen Grenzwert $-\infty$:

$
\lim \limits_{x \to x_0} f(x) = -\infty \quad oder \quad f(x) \overset{ x \rightarrow x_0 }{\longrightarrow} -\infty
$

## Grenzwerte für $x \rightarrow \pm \infty$

Der ***Grenzwert*** der Funktion $y=f(x)$ für $x \rightarrow \infty$ existiert und ist gleich $y_0$, wenn für alle $\epsilon > 0$ ein $M$ existiert, so dass gilt:

$
x > M \Rightarrow |f(x) - y_0| < \epsilon
$

Schreibweisen für den Grenzwert für $x \rightarrow \infty$:

$
\lim \limits_{x \to \infty} f(x) = y_0 \quad oder \quad f(x) \overset{ x \rightarrow \infty}{\longrightarrow} y_0
$

<!-- test -->

Der ***Grenzwert*** der Funktion $y=f(x)$ für $x \rightarrow -\infty$ existiert und ist gleich $y_0$, wenn für alle $\epsilon > 0$ ein $M$ existiert, so dass gilt:

$
x < M \Rightarrow |f(x) - y_0| < \epsilon
$

Schreibweisen für den Grenzwert für $x \rightarrow -\infty$:

$
\lim \limits_{x \to \infty} f(x) = y_0 \quad oder \quad f(x) \overset{ x \rightarrow -\infty}{\longrightarrow} y_0
$

Schreibweise der uneigentlichen Grenzwerte für $x \rightarrow \pm \infty$

$
\lim \limits_{x \to \infty} f(x) = +\infty \quad oder \quad f(x) \overset{x \rightarrow \infty}\longrightarrow +\infty \\
\lim \limits_{x \to \infty} f(x) = -\infty \quad oder \quad f(x) \overset{x \rightarrow \infty}\longrightarrow -\infty \\
\lim \limits_{x \to -\infty} f(x) = +\infty \quad oder \quad f(x) \overset{x \rightarrow -\infty}\longrightarrow +\infty \\
\lim \limits_{x \to -\infty} f(x) = -\infty \quad oder \quad f(x) \overset{x \rightarrow -\infty}\longrightarrow -\infty
$

## Grenzwerte elementarer Funktionen

### Potenzfunktionen ($x^n; x^{-n}$)

$
\lim \limits_{x \to \infty} x^n = \infty
$

## Rechnen mit Grenzwerten

## Stetigkeit