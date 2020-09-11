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

$
"\infty^n " = \infty
$

$
\lim \limits_{x \to \infty} \frac{1}{x^n} = 0
$

$
"\frac{1}{\infty}" = 0
$

$
\lim \limits_{x \to \infty} x^n = 0
$

$
"0^n " = 0
$

$
\lim \limits_{x \to \infty^+} \frac{1}{x^n} = \infty
$

$
"\frac{1}{0^+}" = \infty
$

$
\lim \limits_{x \to \infty^+} \frac{1}{x^n} = 
\begin{cases}
+\infty & \text{falls n gerade} \\
-\infty & \text{falls n ungerade}
\end{cases}
$

$
"\frac{1}{0^-}" = -\infty
$

### Exponentialfunktionen ($e^x; a^x$)

$
\lim \limits_{x \to \infty} e^x = \lim \limits_{x \to -\infty} e^{-x} = \infty
$

$
"e^\infty" = \infty
$

$
\lim \limits_{x \to -\infty} e^x = \lim \limits_{x \to \infty} e^{-x} = 0^+
$

$
"e^{-\infty}" = 0^+
$

$
\lim \limits_{x \to \infty} e^x = \lim \limits_{x \to \infty} e^{-x} = 1
$

$
"e^0" = 1
$

$
\lim \limits_{x \to \infty^+} a^x = 
\begin{cases}
0 & \text{für 0 < a < 1} \\
1 & \text{für a = 1} \\
\infty & \text{für a > 1}
\end{cases}
$

$
\lim \limits_{x \to \infty^+} a^x = 
\begin{cases}
\infty & \text{für 0 < a < 1} \\
1 & \text{für a = 1} \\
0 & \text{für a > 1}
\end{cases}
$

### Logarithmusfunktionen ($ln x$ und $log_a$ mit $a>1$) 

$
\lim \limits_{x \to \infty}{(ln x) = \infty}
$

$
\lim \limits_{x \to 1}{(ln x) = 0}
$

$
\lim \limits_{x \to 0^+}{(ln x) = -\infty}
$

### Sonstige elementare Grenzwerte

$
\lim \limits_{x \to \infty}{(1 + \frac{1}{x})^x} = \lim \limits_{x \to 0^+}{(1 + x)^\frac{1}{x} = e}
$

$
\lim \limits_{x \to \infty}{(1 - \frac{1}{x})^x} = \lim \limits_{x \to 0^+}{(1 - x)^\frac{1}{x} = \frac{1}{e}}
$

$
\lim \limits_{x \to \infty}{\frac{x^n}{e^x}} = 0 (n \in \mathbb{R})
$

<!-- ## Rechnen mit Grenzwerten -->

## Stetigkeit

Eine Funktion $y = f(x)$ heißt an der Stelle $x_0$ ***stetig***, wenn ihr Grenzwert dort existiert und gleich dem Funktionswert an dieser Stelle ist:

$
\lim \limits_{x \to x_0}{f(x) = f(x_0)}
$

Eine Funktion $f_x$ heißt an der Stelle $x_0$ ***rechtseitig stetig***, wenn ihr rechtsseitiger Grenzwert dort existiert und gleich dem Funktionswert an dieser Stelle ist:

$
\lim \limits_{x \searrow x_0}{f(x) = f(x_0)}
$

Eine Funktion $f_x$ heißt an der Stelle $x_0$ ***linksseitig stetig***, wenn ihr linksseitiger Grenzwert dort existiert und gleich dem Funktionswert an dieser Stelle ist:

$
\lim \limits_{x \nearrow x_0}{f(x) = f(x_0)}
$