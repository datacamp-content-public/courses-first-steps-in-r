---
title: 'Teaching Case: Verkaufsgruppenanalyse'
description: 'Das Unternehmen XY.'
---

## Käuferanalyse: Vorstellung Unternehmen XY

```yaml
type: VideoExercise
key: b55ea9901e
xp: 50
```

`@projector_key`
6b5aa056d6283392bbe5e5d08d0bb795

---

## Hands-on R: Lasst uns anfangen

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

Datensätze können in R auf verschiedenste Weise importiert werden. Um Daten aus Exceltabellen und csv-Dateien zu importieren, gibt es zwei gängige Methoden: 

1) read.csv 	(Komma 		(,) separierte Dateien)
2) read.csv2 	(Semikolon  (;) separierte Dateien)

Zuerst lese das zu bearbeitende Datenset "Verkaufsdaten" ein. (Auszug hier der Datei)

`@hint`
Nutze die Funktion #read.csv2() 
(liest externen Datensatz ein)

`@pre_exercise_code`
```{r}
ShowerPath <- "https://assets.datacamp.com/production/repositories/4810/datasets/92686befd7e2045e704ac3f441df3e5ddddbd2f4/Shower_data.csv"
```

`@sample_code`
```{r}

```

`@solution`
```{r}
read.csv2(ShowerPath)
```

`@sct`
```{r}

```
