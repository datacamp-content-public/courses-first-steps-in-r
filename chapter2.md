---
title: 'Case: Verkaufsgruppenanalyse'
description: 'Das Unternehmen XY'
---

## Hands-on R: Lasst uns anfangen

```yaml
type: NormalExercise
key: 8b850e45ae
xp: 100
```

Erste Schritte, um R 'hands-on' zu lernen und die interaktive Programmierumgebung kennenzulernen.
Hier sehen Sie den Data Science Zyklus. Diesen werden wir Schritt für Schritt anhand eines kleinen Datensatzes von Kundendaten aus drei Informationssystemen der Firma XY durchgehen.

![1](https://assets.datacamp.com/production/repositories/4810/datasets/82d92f41d7649657073e1e2e0b813011ecc4973a/Data_Science_Explore.png)

(Quelle: Wickham/Grolemund 2018, S.XI)

`@instructions`
Willkommen in der Programmierumgebung DataCamp. Lasst uns nun direkt mit dem Datensatz loslegen. 

Hier Vorgeschichte Datenset + Problemstellung + Was macht ein DataScientist
Zuerst lese das zu bearbeitende Datenset "Shower_Data" ein, dass durch Semikola getrennte Spalten enthält!

`@hint`
Nutze die Funktion #read.csv2() 
(liest externen Datensatz ein)

`@pre_exercise_code`
```{r}
read.csv2("https://assets.datacamp.com/production/repositories/4810/datasets/92686befd7e2045e704ac3f441df3e5ddddbd2f4/Shower_data.csv")
```

`@sample_code`
```{r}

```

`@solution`
```{r}

```

`@sct`
```{r}
# sct code
# first instruction
test_object("", incorrect_msg = "Something is wrong with `my_vect`. Take another look at the instruction.")

# second instruction
test_object("", incorrect_msg = "Something is wrong with `my_mean`. The easiest way to complete this instruction is to use the `mean()` function with `my_vect`.")
test_function("mean")

# third instruction
test_output_contains("", incorrect_msg = "Take a look at your code for the third instruction. To calculate the sum of squares you will need to take the sum of the square of the difference between `my_vect` and `my_mean`.")
test_function("sum")

# General
test_error()
success_msg("Good job! You've learned some very important and useful functions in this course. Writing SCT's can get complex, but mastering the functions covered in this exercise will get you started so that you can begin creating your own content.")
```
