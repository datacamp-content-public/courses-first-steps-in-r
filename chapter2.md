---
title: 'Teaching Case: Kundendaten analysieren'
description: 'Das Unternehmen XY.'
---

## Problemstellung

```yaml
type: VideoExercise
key: 570b5b662b
xp: 50
```

`@projector_key`
32f5909bd9725fdcbf4b5ffeb2ee4f3f

---

## Lasst uns anfangen: Daten einlesen

```yaml
type: NormalExercise
key: 8b850e45ae
xp: 100
```

Erste Schritte, um R 'hands-on' zu lernen und anzuwenden.
Hier sehen Sie den Data Science Zyklus. Diesen werden wir Schritt für Schritt anhand der Datensätze von Kundendaten aus zwei verschiedenen Datenbanken des Informationssystems der Firma XY durchgehen.

![1](https://assets.datacamp.com/production/repositories/4810/datasets/82d92f41d7649657073e1e2e0b813011ecc4973a/Data_Science_Explore.png)

(Quelle: Wickham/Grolemund 2018, S.XI)

`@instructions`
Willkommen in der Programmierumgebung DataCamp. Lasst uns nun direkt mit dem Importieren der Datensätze loslegen. 

Datensätze können in R auf verschiedenste Weise importiert werden. Um Daten aus Exceltabellen, die als csv-Dateien abgespeichert werden und csv-Dateien zu importieren, gibt es zwei gängige Möglichkeiten: 

1) read.csv 	(Komma 		(,) separierte Dateien)

2) read.csv2 	(Semikolon  (;) separierte Dateien)

Zuerst lese das zu bearbeitende Datenset **Kundendaten** ein.

`@hint`
Nutze die Funktion #read.csv() (liest externen Datensatz ein, der mit Komma separiert ist)

`@pre_exercise_code`
```{r}
Kundendaten <- "https://assets.datacamp.com/production/repositories/4810/datasets/10696eb6afd691cd79a8537c8ae6f300af7ecea5/Kundendaten1.csv"
```

`@sample_code`
```{r}

```

`@solution`
```{r}
read.csv(Kundendaten)
```

`@sct`
```{r}

```

---

## Daten erkunden

```yaml
type: TabExercise
key: cac9b34188
xp: 100
```

Schauen Sie sich die Daten zuerst an und verschaffen Sie sich einen Überblick, was an Datentypen und Werten vorliegt.

Nützliche Funktionen für die Datenerkundung in R sind:
- **nrow()** | **ncol()**: nrow and ncol gibt die Anzahl der Zeilen und Spalen in x zurück. Nrow und ncol behandeln einen Vektor genauso wie eine 1-spaltige Matrix.
- **names()**: Funktionen zum Abrufen oder Einstellen der Namen eines Objekts.
- **colnames()**: Abrufen oder setzen der Zeilen- oder Spaltennamen eines matrixartigen Objekts.
- **head()** | **tail()**: Liefert den ersten oder letzten Teil eines Vektors, einer Matrix, einer Tabelle, eines Datenrahmens oder einer Funktion.
- **summary()**: Ist eine generische Funktion, um Ergebniszusammenfassungen zu erstellen.

(Quelle: R Dokumentation)

`@pre_exercise_code`
```{r}
Kundendaten <- "https://assets.datacamp.com/production/repositories/4810/datasets/10696eb6afd691cd79a8537c8ae6f300af7ecea5/Kundendaten1.csv"
```

***

```yaml
type: NormalExercise
key: f5a76cb84c
xp: 100
```

`@instructions`
Wie viele Zeilen gibt es? Wie viele Spalten sind im Datensatz vorhanden?

`@hint`
Nutzen Sie bitte die Funktionen nrow() und ncol()

`@sample_code`
```{r}
# 1.Wie viele Zeilen gibt es?

# 2.Wie viele Spalten gibt es?

```

`@solution`
```{r}
# 1.Wie viele Zeilen gibt es?
nrow("Kundendaten")
# 2.Wie viele Spalten gibt es?
ncol("Kundendaten")
```

`@sct`
```{r}

```

***

```yaml
type: NormalExercise
key: 580db0e321
```

`@instructions`
Jetzt wissen Sie, wie groß der Datensatz ist. Verschaffen Sie sich bitte einen Überblick über die größten oder kleinsten Werte, die in den Kundendaten enthalten sind, um mögliche Ausreißer, besonders profitable bzw. unprofitable Kunden zu identifizieren.

`@hint`
Nutzen Sie die Funktionen head() und tail()

`@sample_code`
```{r}
# Größsten Werte

# -> Schauen Sie sich bitte den Datensatz in der Console an und merken Sie sich bitte Auffälligkeiten

# Kleinsten Werte

# -> Was fällt Ihnen hier im Datensatz auf?

```

`@solution`
```{r}
# Größsten Werte
head(Kundendaten)
# Kleinsten Werte
tail(Kundendaten)
```

`@sct`
```{r}

```

***

```yaml
type: NormalExercise
key: 968ce3981c
```

`@instructions`
Wir sind immer noch in dem Schritt, die Daten genau zu erkunden, um eine Überblick zu gewinnen und zu schauen, in welcher Qualität die Daten vorliegen. Welche der Funktionen, die vorgestellt wurden, eignen sich dafür zum Abschluss noch?

`@hint`
Um Ergebniszusammenfassungen zu bekommen eigent sich die Funktion: summary()

`@sample_code`
```{r}
# Gesamtüberblick
```

`@solution`
```{r}
# Gesamtüberblick
summary(Kundendaten)
```

`@sct`
```{r}

```

---

## Check: Auffälligkeiten entdeckt?

```yaml
type: PureMultipleChoiceExercise
key: 47a850ee0f
xp: 50
```

Der Chef von Ihnen fragt Sie, ob Sie Auffälligkeiten entdeckt haben oder der Datensatz zu weiteren Analyse schon verwendbar sei.
Was sagen Sie Ihm?
Achtung: Es ist nur **eine** Möglichkeit richtig! Lesen Sie bitte genau und wählen danach eine Antwort aus.

- 1 : Ja, der Datensatz Kundendaten ist für die Analyse fertig bereinigt und enthält keine Auffälligkeiten
- 2 : Nein, es sind fehlende Werte enthalten
- 3 : Nein, es gibt Ausreißerwerte bei dem Umsatz, die kommen mir nicht realistisch vor.
- 4 : Nein, es gibt unrealistische Werte bei dem Umsatzdaten einzelner Kunden und es sind fehlende Werte im Datensatz enthalten.
- 5 : Sorry Chef, ich habe keinen Überlick gewonnen und bin mir nicht sicher.

`@hint`


`@possible_answers`
- 1
- 2
- 3
- [4]
- 5

`@feedback`
- "Nein, da haben Sie viele Werte und Auffälligkeiten übersehen. Sie müssen genauer arbeiten.
- "Nein. Sie liegen schon richtig, nur haben Sie eine Kombination übersehen. Es liegen zusätzlich Umsatzausreißer vor."
- "Nein. Sie liegen schon richtig, nur haben Sie eine Kombination übersehen. Es liegen zusätzlich fehlende Werte vor."
- "Ja, sehr gut! Sie haben sehr aufmerksam die Daten erkundet."
- "Naja, dann aber beim nächsten mal bitte genauer!""

---

## Daten bereinigen

```yaml
type: NormalExercise
key: a446c3e473
xp: 100
```

Das Aufräumen bzw. **Bereinigen** Ihrer Daten bedeutet, sie in einer konsistenten Form zu speichern, die der Semantik des Datensatzes mit der Art der Speicherung entspricht. Kurz gesagt, wenn Ihre Daten bereinigt sind, ist jede Spalte eine Variable und jede Zeile ist eine Beobachtung. Das Bereinigen (tyding) ist wichtig, weil die einheitliche Struktur es Ihnen ermöglicht Ihren Fokus auf die Fragen zu den Daten zu konzentrieren. 
(Quelle: Wickham/Grolemund 2018, S.X)

`@instructions`


`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}

```

`@sct`
```{r}

```

---

## Transformieren

```yaml
type: NormalExercise
key: 8767c4d2d3
xp: 100
```

Der nächste übliche Schritt nach der Bereinigung der Daten (Tidying) ist es, die Daten zu **transformieren**. Dazu gehört die Einschränkung des Datensates auf das Analyseinteresse, die Erstellung neuer Variablen, die Funktionen bestehender Variablen sind und die Berechnung eines Satzes von zusammenfassenden Statistiken (counts, means, ...)
(Quelle: Wickham/Grolemund 2018, S.X)

`@instructions`


`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}

```

`@sct`
```{r}

```

---

## Visualisieren

```yaml
type: NormalExercise
key: 78c1c653dc
xp: 100
```

Die **Visualisierung** ist eine grundlegende menschliche Aktivität und zeigt Ihnen Erkenntnisse, die Sie nicht erwartet hatten oder lässt Sie neue Fragen an die Daten stellen.Eine gute Visualisierung könnte auch darauf hinweisen, dass Sie die falschen Fragen stellen oder dass Sie andere Daten sammeln müssen. Die Visualisierung lässt Sie Daten besser interpretieren, jedoch skaliert sie nicht immer gut, da sie von Menschen in den häuftisgten Fällen für kontextbasierte und individuelle Sachverhalte angefragt wird.
(Quelle: Wickham/Grolemund 2018, S.X)

`@instructions`


`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}

```

`@sct`
```{r}

```

---

## (Modellieren)

```yaml
type: NormalExercise
key: 2a50556aeb
xp: 100
```

Modelle sind ergänzende Werkzeuge zur Visualisierung. Wenn Sie Ihre Fragen ausreichend präzise (mathematisch) formuliert haben, können Sie sie mit einem Modell beantworten. Modelle skalieren den Wert, weil sie Rechenwerkzeuge sind. Aber jedes Modell beinhaltet Annahmen und von Natur aus kann ein Modell seine eigenen Annahmen nicht in Frage stellen. Das bedeutet, dass ein Model Sie nicht fudamental überraschen kann.
(Quelle: Wickham/Grolemund 2018, S.X)

`@instructions`


`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}

```

`@sct`
```{r}

```

---

## Welche Erkenntnisse durch die Datenanalyse haben Sie gewonnen?

```yaml
type: PureMultipleChoiceExercise
key: 64b02c906d
xp: 50
```



`@hint`


`@possible_answers`


`@feedback`


---

## Kommunizieren: Führungskräftemeeting

```yaml
type: PureMultipleChoiceExercise
key: fa8fdf9d03
xp: 50
```

Der letzte Schritt eins Data Science Projektes ist die **Kommunikation**. Ein absolut erfolgskritischer Teil eines jeden Datenanalyseprojektes. Es spielt keine Rolle, wie gut Ihre Modelle und Visualisierungen Sie dazu gebracht haben, die Daten zu verstehen, es sei denn, Sie können die Ergebnisse auch an andere verständlich weitergeben und (ökonomischen) Wert damit generieren.
(Quelle: Wickham/Grolemund 2018, S.X)

`@hint`


`@possible_answers`


`@feedback`
