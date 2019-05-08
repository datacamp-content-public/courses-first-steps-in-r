---
title: 'Teaching Case: Verkaufsgruppenanalyse'
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
Hier sehen Sie den Data Science Zyklus. Diesen werden wir Schritt für Schritt anhand der Datensätze von Kundendaten aus drei verschiedenen Datenbanken des Informationssystems der Firma XY durchgehen.

![1](https://assets.datacamp.com/production/repositories/4810/datasets/82d92f41d7649657073e1e2e0b813011ecc4973a/Data_Science_Explore.png)

(Quelle: Wickham/Grolemund 2018, S.XI)

`@instructions`
Willkommen in der Programmierumgebung DataCamp. Lasst uns nun direkt mit dem Importieren der Datensätze loslegen. 

Datensätze können in R auf verschiedenste Weise importiert werden. Um Daten aus Exceltabellen und csv-Dateien zu importieren, gibt es zwei gängige Möglichkeiten: 

1) read.csv 	(Komma 		(,) separierte Dateien)

2) read.csv2 	(Semikolon  (;) separierte Dateien)

Zuerst lese das zu bearbeitende Datenset **Kundendaten** ein.

`@hint`
Nutze die Funktion #read.csv() (liest externen Datensatz ein, der mit Semikolons separiert ist)

`@pre_exercise_code`
```{r}
Kundendaten <- "https://assets.datacamp.com/production/repositories/4810/datasets/400b53fb59ceec79beddacd8a9ea615f0f0df336/Kundendaten.csv"
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
- **summary()**: Ist eine generische Funktion, um Ergebniszusammenfassungen der Ergebnisse verschiedener Modellanpassungsfunktionen zu erstellen.
(Quelle: R Dokumentation)


`@pre_exercise_code`
```{r}
Kundendaten <- "https://assets.datacamp.com/production/repositories/4810/datasets/400b53fb59ceec79beddacd8a9ea615f0f0df336/Kundendaten.csv"
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
Jetzt wissen Sie, wie groß der Datensatz ist. Verschaffen Sie sich bitte einen Überblick über die größten und kleinsten Werte, die in den Kundendaten enthalten sind, um mögliche Ausreißer, besonders profitable bwz. unprofitable Kunden zu identifizieren.

`@hint`
Nutzen Sie die Funktionen head() und tail()

`@sample_code`
```{r}
# Größsten Werte

# Kleinsten Werte

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

---

## Daten bereinigen

```yaml
type: NormalExercise
key: a446c3e473
xp: 100
```



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



`@hint`


`@possible_answers`


`@feedback`
