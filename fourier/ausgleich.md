# Ausgleichsvorgänge

## Schaltvorgänge im Zeitbereich

In diesem Abschnitt sollen Vorgäng betrachtet werden, die sich gerade durch zeitliche Veränderungen auszeichnen. Man spricht von **Ausglichsvorgängen** und meint damit die Situation in einer Schaltung, die sich nach einer schlagartigen Änderungen des Eingangssignals ergibt. Das is bspw. der Fall, wenn der Eingang der Schaltung zum ersten Mal an eine Spannung angeschlossen wird oder wenn sich der Spannungswert gerade sprunghaft verändert hat. Dann werden eventuell vorhandene Kondensatoren oder Induktivitäten erst noch auf- oder umgeladen, bevor erneut ein eingeschwungener Zustand, nun aber mit anderen Werten von Strömen und Spannungen, vorliegt.

Der Grundgedanke zu Ausgleichsvorgängen. In einer auf die Spannung $U$ aufgeladenen Kapazität ist bekanntlich eine Energie der Größe $W_C$ gespeichert, für die gilt:

$$W_C=\frac{1}{2}C\cdot U^2$$

Analog beträgt die in einer von einem Strom $I$ durchflossenen Induktivität gespeicherte Energie:

$$W_L=\frac{1}{2}L\cdot I^2$$

Bei einer Spannungsänderung an der Kapazität ändert sich somit auch die gespeicherte Energie. Sprunghafte Änderungen würde bedeuten, dass

$$\frac{dW_C}{dt} \rightarrow \infty$$

und

$$\frac{dW_L}{dt} \rightarrow \infty$$

Das ist aber physikalisch unmöglich, denn die Ableitung der Energie nach der Zeit ist nichts anderes als die Leistung. Das bedeutet, dass man für eine sprunghafte Änderung der Energie unednlich große Leistung bräucthe - was natürlich nicht möglich ist. Die Konsequenz daraus lautet:

> Energiespeicher wie Kapazität und Induktivität können Änderungen ihres Ladezustands nur unter kontinuierlichem Verlauf von $U$ beziehungszweise $I$ realisieren.

---

**Quelle: [Wikipedia](https://de.wikipedia.org/wiki/Ausgleichsvorgang)**

### Ausgleichsvorgang

Ein Ausgleichsvorgang tritt in einem physikalischen oder chemischen System auf, in dem ein stationärer Vorgang durch einen Eingriff-- wie etwa Einschalten, Belastungsänderung, Störung im Prozess - verändert wird und in einen neuen stationären Vorgang übergeht.

Ausgleichsvorgänge sind von allgemeiner physikalischer Bedeutung und treten in vielen technischen Vorgängen auf. Sie erfolgen nicht Sprunghaft zum Zeitpunkt des Eingriffs, sondern stetig und werden durch das Zeitverhalten bestimmter Zustandgrößen beschrieben. Bspw. in der Elektrotechnik beim Ladevorgang eines Kondensators kann als diese Zustandgröße die Spannung dienen.

Es ist im allgemeinen Fall nicht selbstverständlich, dass ein Ausgleichsvorgang in einen stabilen, stationären Vorgang übergeht.  

### Ursache, Verlauf

Physikalische Ursache eines Ausgleichsvorgangs ist die in Bauteilen gespeicherte Energie oder Masse, die nicht sprunghaft geändert werden kann. Bspw. in der Elektrotechnik handelt es sich um elektrische Energie in Kapazitäten, magnetische Energie in Induktivitäten und Rotationsenergie in rotierenden Maschinen. Das Ergebnis des Ausgleichsvorgangs ist ein neuer Dauervorgang. Bei zu Schwingungen fähigen Systemen (bspw. Wechselstromnetz) wird der stationäre Vorgang dadurch charakterisiert, dass Amplitude und Frequenz aller sinusförmigen Zustandsgrößen konstant sind.

Der Ausgleichsvorgang kann aperiodisch (gleitend) oder schwingend verlaufen, so dass der Endzustand auch als eingeschwungener Zustand bezeichnet wird. Im Ausgleichsvorgang kann es beispielswiese in einem Wasserrohr durch Rohrbruch (oder Pumpenausfall) tortz der damit verbundenen Druckabsenkung gleichwohl zu unzulässig hohen Druckstößen kommen, die weitere Rohrbruche auslösen.

Bei einem schwingenden Vorgang is das Ausmaß des Ausgleichsvorgangs nicht vorhersehbar, da sein Anfangszustand durch die Zufälligkeits des Zeitpunktes des Eingriffs ungewiss ist. Insbesonder bei Wechselstromkreisen können von Zeitpunkt (Phasenwinkel) abhängige beträchtliche Spannungs- oder Stromüberhöhungen enstehen bei höherer Frequenz als Netzfrequenz, siehe beispielsweise Frequenzanganben zum Erdschluss. Der neue stationäre Vorgang ist dagegen vom Anfangszustand unabhängig.

### Mathematische Behandlung

Die mathematische Behandlung von Ausgleichsvorgängen führt auf eine lineare gewöhnliche Differentialgeichung mit konstanten Koeffizienten. Bei $n$ Speicherelementen ist diese von $n$-ter Ordnung. Alternativ sind $n$ Differentialgleichen erster Ordnung möglich. Ihre Lösung beschreibt eine Überlagerung des zu erwartenden neuen eingeschwungenen Vorgangs und des asymptotisch abklingenden (flüchigen) Ausgleichsvorgangs. Bspw. bei einem Stromkreis kann der Strom als Überlagerung eines stationären Stromes und eines Ausgleichsstromes beschrieben werden, der den stetigen Übergang vermittelt.

- Der stationäre Vorgang folgt aus der partikulären Lösung der inhomogenen Differentialgleichung für $t \rightarrow \infty$. In der Elektrotechnik entspricht das einer Gleichstrom- oder Wechselstromrechnung.

- Der flüchtiger Vorgang folgt aus der allgemeinen Lösung der homogenen Differentialglichung einschließlich Konstantenbestimmung.

Alternative können die Differnetialgleichungen mit Hilfe der Laplace-Transformation gelöst werden. Differenzieren und Integrieren werden durch diese Transformation auf Multiplizieren und Dividieren zurückgeführt. Aus einer linearen Differentialgleichung im Zeitbereich wird eine lineare algebraische Gleichung in einem Bildbereich.

---

## RC-Serienschaltung

### Grundzusammenhänge

Man betracthe die in der Abbildung dargestellte Schaltung. Aus Gründen, die später klar werden, bezeichnet man diese Anordnung auch als ein RC-Integrierglied oder einen RC-Tiefpass.

```{figure} ../images/abb1.png
---
scale: 50%
align: center
---
RC-Stromkreis
```

Ein Kondensator $C$ in Serie mit einem Widerstand $R$ ist über einen Schalter an einen Konstantspannungsquelle $U$ angeschlossen. Der Schalter wird genau im Zeitpunk $t=0$ geschlossen. Der Kondensator sei im Moment des Einschaltens noch entladen ($u_C = 0$). Nach dem Schließen des Schalters wird natürlich Strom fließen, der im ersten Augenblick den Betrag $i(t=0)=U/R$ hat. Man stellt also fest:

> Im Moment des Einschaltens verhält sich eine ungeladene Kapazität wie ein Kurzschluss.

Der fließende Strom lädt nun den Kondensator auf, sodass $u_C(t)$ ansteigt. Der Stromfluss wird mit zunehmendem $u_C$ immer schwächer, denn die über $R$ liegende Spannung $U - u_C$ nimmt ab und somit auch der durch $R$ über das ohmsche Gesetz erzwungene Strom. Wenn $u_C$ den Wert von $U$ erreicht hat, verisegt der Stromfluss schließlich ganz - der Kondensator ist aufgeladen und der Ausgleichsvorgang ist somit abgeschlossen. 

---
**Quelle: [Wikipedia](https://de.wikipedia.org/wiki/RC-Glied)**

Unter RC-Gliedern versteht man in der Elektrotechnik Schaltungen, die aus einem ohmschen Widerstand (R- engl. resistor) un einem Kondensator (C - engl. capacitor) aufgebaut sind. RC-Glieder sind lineare, zeitinvariante Systeme. Im engeren Sinne sind damit die Filter wie der Tiefpass oder Hochpass gemeint. Bei einem Tiefpass, wie im nebenstehenden Bild, ist der Kondensator parallel am Signalausgang geschaltet, beim Hochpass sind Kondensator und Widerstand vertauscht.

Zum Potentialausgleich beziehungswiese bei der Funktionserdung finden sich Parallelschaltungen von Konensator und Widerstand. Zur Begrenzung von elektromagnetischen Störungen finden sich Reihenschaltungen von Kondensator und Widerstand, wie beispielsweise bei dem Snubber.

```{figure} ../images/abb2.png
---
scale: 50%
align: center
---
Einfacher RC-Tiefpass $U_e$: Eingangsspannung $U_a$: Ausgangsspannung
```

### Snubber

**Quelle: [Wikipedia](https://de.wikipedia.org/wiki/Snubber)**

Das aus dem technischen Englisch stammende Wort **Snubber** umschreibt eine Einrichtug zur Dämpfung unerwünschter Schwinungungen in technischen Anwendungen.

Am häfugisten wird der Begriff in der Elektronik verwendet. ***Snubber*** können aber auch mechanische Schwningungsdämpfer, beispielsweise Stoßdämpfer, Kettendämpfer oder Lenkungsdämpfer, sowie hydraulisch/pneumatische Pulsationsdämpfer oder Schalldämpfer sein, bei diesen Anwendungen ist der Begriff jedoch weniger gebräuchlich. 

### Elektrische Snubber

Als ***Snubber-Glied*** bezeichnet man eine elektrische Schaltung, die störende Hochfrequenzen oder Spannungsspitzen neutralisieren soll, die meist beim Schalten induktiver Lasten auftreten, wenn der Stromfluss abrupt unterbrochen wird. Es wird zur Erreichung einer besseren elekromagnetischen Verträglichkeit, zur Funkenlöschung an Schaltkontakten und zur Begrenzung der Spannungsanstiegsgeschwindigkeit an Halbleiterschaltern (Thyristoren, IGBT, Bipolartransistoren) eingesetzt.

### Verwendung

Snubberglieder werden beispielswiese an Kontakten von Leistungsrelais, Schützen und anderen elektrischen Kontakten eingesetzt, wenn diese induktive Lasten zu schalten haben. Beim Prellen und Öffnen der Kontakte in einem Stromkreis, der Induktivitäten enthält, entsteheen ohne Kondensator steile Spannungsspitzen, weil die Änderungsgeschwindigkeit des Stroms groß ist. Diese Spannungsspitzen werden durch einen Snubber abgefangen und gedämpf, wei die Stromänderungsgeschwindigkeit verkleinert wird: Der Strom fließt beim Abschalten zunächst in der ursprünglichen Höhe statt über die Kontakte in den Kondensators entsprechend der abnehmenden amgnetischen Energie ab. Gleichzeitig wird durch den Stromfluss im Widerstand elektrische Energie in Wärme umgewandelt, die sonst zu einer Resonanzschwingung führen würde. Dadurch gelingt es, Funkenentladungen zu vermeiden und die Kontaktlebensdauer wesentlich zu erhöhen. Weiterhin wird die Emission von Funkstörungen stark verringert. Beim Wiedereinschalten sorgt de rWiderstand dafür, dass der Einschaltstrom beim Entladen des Kondensators begrenzt wird.

Eine weitere Aufgabe von Snubbergliedern ist die Begrenzung der Spannungsanstiegs-Geschwindigkeit an Halbleitern auf einen für diese unkritischen Wert. Thyristoren/Triacs zeigen ansonsten ein unerwünschtes Überkopfzünden. IGBTs und Bipolartransistoren können sogar zerstört werden. Bei MOSFETs führt die Miller-Kapazität bei zu schnellem Spannungsanstieg zu unsauberem Ausschaltverhalten und erhöhrten Schaltverlusten.

Am Lautsprecherausgang einer Audioverstärkerschaltung sorgt ein oft externes Snubberglied dafür, dass der Verstärker an der induktiv-komplexen Last einer Lautsprecherbox stabil arbeitet und keine sogenannten "wilden" Schwingungen ausführt. Die Wirkung beruht zum einen darauf, dass der induktive Impedanzanstieg der angeschlossenen Lautsprecher bei hohen NF-Frequenzen durch den gegenläufigen Impedanzabfall des Snubbergliedes teilweise kapazitiv kompensiert wird und der Verstärker somit über seinen Arbeitsfrequenzbereich etwa den gleichen reellen Lastwiderstand vorfindet, was dann insgesamt die Stabilität (=Schwingfreiheit) des NF-Verstärkers zusammen mit seinen Gegenkopplungsgliedern erhöht. Oberhalb von etwa 20kHz wirkt das Boucherot-Glied bei klein gewähltem Boucherot-Widerstand zunehmend als Kurzschluss für das Ausgangssignal und wirkt damit ähnlich wie ein Frequenzkompensation (=Grenzfrequenzbegrenzung) beim Operationsverstärker, wobei der Amplitudenabfall am Ausgang stärker als der Signallaufzeiteinfluss des Verstärkers ist, der sich durch den frequenzabhängigen Phasenwinkel zwischen Ein- und Ausgangssignal ausdrückt. D.h. keine Signalfrequenz innerhalb des Arbeitsfrequenzbereiches und etwas darüber findet über die verstärkungsfestlegenden externen und internen Gegenkopplungen des Verstärkers eine Mitkopplungsbedingung vor, die sonst sofort die gefürchtete Selbsterregung ("wilde" Schwingung) erzeugen könnte.

### Funktionswiese

Beim Öffnen eines Schalters (Kontakt oder Halbleiterbautiel), an den ein induktiver Verbraucher angeschlossen ist, entsteht ohne geeignete Beschaltung ein steiler Spannungsantieg bis zum Durchbruch (Schaltlichtbogen oder Avalanchedurchbruch), weil die Induktivität eine hohe Spannung erzeugt, da sie bestrebt ist, den Stromfluss aufrechtzuerhalten.

Der Kondensator des Snubbergliedes übernimmt beim Öffnen des Kontaktes temporär den Stromfluss, so dass der Schalter ohne Funken bzw. mit begrenzter Spannungsanstiegsgeschwindigkeit öffnet.

Der Widerstand hat zwei Aufgaben:

- Dämfung des HF-Schwingungen
- Begrenzung des Ladestromes des Kondensators beim Schließen des Schalters

Nachteil: Im geöffneten Zustand fließt bei Wechselstrom, bedingt durch den Wechselstromwiderstand (Impedanz) des Kondensators, immer ein Strom durch den Snubber und den Verbraucher. Das kann in einigen Fällen vermieden werden, indem das Snubberglied direkt über den (induktiven) Verbraucher geschaltet wird. Da in diesem Fall die Impedanz des speisenden NEtzes in Reihe liegt (das Niederspannungsnetz ist meist induktiv!), verringert sich die Entstörwirkung. Das kann durch einen weiteren, über die Speisequelle geschalteten Kondensator (sog. "X-Kondensator", oft Bestandteil des Netzfilters) vermieden werden. 

---

### Messtechnische Betrachtungen

Für die Messtechnik ist interessant, dass man aus der Vermessung der Aufladekurve die Zeitkonstante $\tau$ und damit bei bekanntem Widerstand $R$ die Kapazität $C$ oder bei bekannter Kapazität $C$ den Widerstand $R$ in einem Schaltkreis bestimmen kann. Dazu gibt es zwei mögliche Vorgehensweisen:

* Steigung im Ursprung

Aus dem Verlauf der Ladespannung lässt sich mittels der Ableitung die Steigung im Ursprung ($t=0$) berechnen:

Das entspricht einer Gerade, die zum Zeitpunkt $t=\tau$ gerde den Wert U erreicht s. Abbildung. Hat man den Spannungsverlauf etwa mit einem Oszilloskop ermittelt, so kann man in die gemessene Kurve die Tangente im ursprung einzeichnen und sie mit der Asymptote für $t \rightarrow \infty$ schneiden. Vom Schnittpunkt geht man senkrecht nach unten und liet $\tau$ ab.

```{figure} ../images/abb3.png
---
scale: 50%
align: center
---
Ermittlung der Zeitkonstanten aus der Aufladekurve über die Steigung bei $t=0$
```

* Funktionswert bei $t=\tau$

Eine andere Möglichkeit, aus der gemessenen Kurve die Zeitkonstante zu bestimmten, ist, den Wert der Kondensatorspannung für $t=\tau$ zu berechnen:

Man nutzt jetzt die Tatsache, dass nach Ablauf der Zeit $\tau$ die Kurve $63\%$ ihres Endwerts erreicht hat, in umgekehrter Richtung. Das heißt, man ermittelt $63\%$ des Endwerts der Kurve, geht horizontal bis zum Schnittpunkt mit der Kurve und von da nach unten zur Zeitache (s. Abbildung). Der gefundene wert is $\tau$. 

```{figure} ../images/abb4.png
---
scale: 50%
align: center
---
Ermittlung der Zeitkonstanten aus der Aufladekurve über den Funktionswert $0,63 \cdot U$
```

Die Zeitkonstante $\tau$ kann man auch aus dem Stromverlauf nach der Abbildung bestimmen. Dann ergeben sich in Analogie zu den gezeigten Vorgehensweisen die folgenden Abbildung 

```{figure} ../images/abb5.png
---
scale: 50%
align: center
---
Ermittlung der Zeitkonstanten aus dem Verlauf des Ladestroms über die Steigung bei $t=0$
```

```{figure} ../images/abb6.png
---
scale: 50%
align: center
---
Ermittlung der Zeitkonstanten aus dem Verlauf des Ladestroms über den Funktionswert $(1-0,63)\cdot U/R$
```

### Aufladung eines Kondensators mit Anfangsladung

Es wird jetzt untersucht, wie die Ladespannung am Kondensator sich etwickelt, wenn der Kondensator bereits eine Anfangsladung enthält, bevor der Schalter geschlossen wird. Die Spannung am Kondensator zum Zeitpunkt $t=0$ betrage also $U=U_{C0}$.

Das heißt, auf die Ladespannung des Kondensators zu Beginn ($U_{C0}$) wird der weitere Ladevorgang einfach "draufgesetzt". Wie man leicht nachvollziehen kann, schließt die eben gewonnene Formel den Fall $U_{C0}=0$ ein.

```{figure} ../images/abb7.png
---
scale: 50%
align: center
---
Zeitverlauf der Ladespannung im RC-Stromkreis mit Anfangsladung des Kondensators
```

### Entladung eines Kondensators

Mit dem Ergebnis des vorigen Abschnitts lässt sich auch der Entladevorgang eines vorher aufgeladenen Kondensators beschreiben. Wir setzen die Spannungsquelle in der Abbildung einfach durch einen Kurzschluss, über den sich der Kondensator entlädt, und erhalten den folgenden dargestellten Stromkreis.

```{figure} ../images/abb8.png
---
scale: 50%
align: center
---
RC-Stromkreis beim Entladevorgang
```

Dieser Zeitverlauf ist in der folgenden Abbildung dargestellt.

```{figure} ../images/abb9.png
---
scale: 50%
align: center
---
Zeitverlauf der Kondensatorspannung bei Entladevorgang
```

### Die Spannung am Widerstand

Bis hierhin stand bei allen Betrachtungen das Verhalten des Kondensators und die dort auftretende Spannung $u_C(t)$ im Mittelpunkt. Jetzt interessiert mehr die Spannung $u_R(t)$ am Widerstand $R$.

Zunächst wird der Aufladevorgang wieder betrachtet. Die Spannung am Widerstand ist die Differenz zwischen der am Eingang anliegenden Spannung $U$ und der Kondensatorspannung $u_C(t)$. Der Verlauf von $u_R(t) ist zusammen mit u_C(t) dargestellt.

```{figure} ../images/abb10.png
---
scale: 50%
align: center
---
Spannungsverläufe $u_R(t) und u_C(t) beim Aufladevorgang im RC-Stromkreis
```


## RL-Serienschaltung

### Grundzusammenhänge

### Messtechnische Betrachtungen

## Übertragung von Rechtecksignalen

### RC-Tiefpass

### RC-Hochpass
