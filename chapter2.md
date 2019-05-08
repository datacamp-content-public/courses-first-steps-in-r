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

Zuerst lese das zu bearbeitende Datenset **ShowerPath** ein. (Auszug hier der Datei)

`@hint`
Nutze die Funktion #read.csv2() (liest externen Datensatz ein, der mit Semikolons separiert ist)

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}
read.csv2(Kundendaten)
```

`@sct`
```{r}

```

---

## Insert exercise title here

```yaml
type: NormalExercise
key: 9ead3b214c
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

Zuerst lese das zu bearbeitende Datenset **Kundendaten** ein. (Auszug hier der Datei)

`@hint`
Nutze die Funktion #read.csv2() (liest externen Datensatz ein, der mit Semikolons separiert ist)

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

## Daten erkunden

```yaml
type: TabExercise
key: cac9b34188
xp: 100
```

Schaue Dir die Daten zuerst an und verschaffe Dir einen Überblick, was an Datentypen und Werten vorliegt.

`@pre_exercise_code`
```{r}
ShowerPath <- "https://assets.datacamp.com/production/repositories/4810/datasets/92686befd7e2045e704ac3f441df3e5ddddbd2f4/Shower_data.csv"
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
