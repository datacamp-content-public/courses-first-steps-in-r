---
title: 'Chapter Title Here'
description: 'Chapter description goes here.'
free_preview: true
---

## Example coding exercise

```yaml
type: NormalExercise
key: 2bafef99a3
lang: r
xp: 100
skills: 1
```

This is an example exercise.

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

## Insert exercise title here

```yaml
type: NormalExercise
key: 1e15c44df4
xp: 100
```

Erste Schritte, um R hands-on zu lernen und die interaktive Programmierumgebung kennenzulernen. 

`@instructions`
Willkommen in der Programmierumgebung DataCamp. Lasst uns direkt loslegen. 

Hier Vorgeschichte Datenset + Problemstellung
Zurerst lese das zu bearbeitende Datenset "Schraenke" ein.

`@hint`
Please use the function # read.csv() (reads comma separated columns)

`@pre_exercise_code`
```{r}
library(dplyr)
read.csv(Schraenke) <- read.csv(https://assets.datacamp.com/production/repositories/4810/datasets/45de207edffda856248885983c45ebfc770147f4/Verkaufsdaten.csv)
```

`@sample_code`
```{r}

```

`@solution`
```{r}
read.csv(Schraenke)
```

`@sct`
```{r}
read.csv(Schraenke)
```
