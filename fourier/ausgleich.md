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

Quelle: Wikipedia

### Ausgleichsvorgang

Ein Ausgleichsvorgang tritt in einem physikalischen oder chemischen System auf, in dem ein stationärer Vorgang durch einen Eingriff-- wie etwa Einschalten, Belastungsänderung, Störung im Prozess - verändert wird und in einen neuen stationären Vorgang übergeht.

Ausgleichsvorgänge sind von allgemeiner physikalischer Bedeutung und treten in vielen technischen Vorgängen auf. Sie erfolgen nicht Sprunghaft zum Zeitpunkt des Eingriffs, sondern stetig und werden durch das Zeitverhalten bestimmter Zustandgrößen beschrieben. Bspw. in der Elektrotechnik beim Ladevorgang eines Kondensators kann als diese Zustandgröße die Spannung dienen.

Es ist im allgemeinen Fall nicht selbstverständlich, dass ein Ausgleichsvorgang in einen stabilen, stationären Vorgang übergeht.  

### Ursache, Verlauf

Physikalische Ursache eines Ausgleichsvorgangs ist die in Bauteilen gespeicherte Energie oder Masse, die nicht sprunghaft geändert werden kann. Bspw. in der Elektrotechnik handelt es sich um elektrische Energie in Kapazitäten, magnetische Energie in Induktivitäten und Rotationsenergie in rotierenden Maschinen. Das Ergebnis des Ausgleichsvorgangs ist ein neuer Dauervorgang. Bei zu Schwingungen fähigen Systemen (bspw. Wechselstromnetz) wird der stationäre Vorgang dadurch charakterisiert, dass Amplitude und Frequenz aller sinusförmigen Zustandsgrößen konstant sind.

Der Ausgleichsvorgang kann aperiodisch (gleitend) oder schwingend verlaufen, so dass der Endzustand auch als eingeschwungener Zustand bezeichnet wird. Im Ausgleichsvorgang kann es beispielswiese in einem Wasserrohr durch Rohrbruch (oder Pumpenausfall) tortz der damit verbundenen Druckabsenkung gleichwohl zu unzulässig hohen Druckstößen kommen, die weitere Rohrbruche auslösen.

Bei einem schwingenden Vorgang is das Ausmaß des Ausgleichsvorgangs nicht vorhersehbar, da sein Anfangszustand durch die Zufälligkeits des Zeitpunktes des Eingriffs ungewiss ist. Insbesonder bei Wechselstromkreisen können von Zeitpunkt (Phasenwinkel) abhängige beträchtliche Spannungs- oder Stromüberhöhungen enstehen bei höherer Frequenz als Netzfrequenz, siehe beispielsweise Frequenzanganben zum Erdschluss. Der neue stationäre Vorgang ist dagegen vom Anfangszustand unabhängig.

---

## RC-Serienschaltung

### Grundzusammenhänge

### Messtechnische Betrachtungen

### Aufladung eines Kondensators mit Aunfangsladung

### Entladung eines Kondensators

### Die Spannung am Widerstand

## RL-Serienschaltung

### Grundzusammenhänge

### Messtechnische Betrachtungen

## Übertragung von Rechtecksignalen

### RC-Tiefpass

### RC-Hochpass
