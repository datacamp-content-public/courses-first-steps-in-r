---
title: 'Wie R funktioniert'
description: "Um die Übung zu lösen, geben Sie im Editor auf der rechten Seite den R-Code ein. Wenn Sie auf den Button \"Submit Answer\" klicken, wird jede Codezeile interpretiert und durch R ausgeführt. Sie erhalten eine Nachricht, ob der von Ihnen erstellte Code richtig war. Ihre Ausgabe des R-Codes wird in der Konsole unten rechts angezeigt.\n\nIn R wird die #-Taste genutzt, um Kommentare zu kennzeichnen, die Ihnen und anderen R-Nutzern zusätzliche Informationen über den Code bereitstellen. Kommentare werden nicht als R-Code ausgeführt, somit beeinflussen sie die Ergebnisse nicht. Zum Beispiel Berechnen Sie 3+4 ist im Editor rechts ein Kommentar.\n\nSie können die R-Befehle auch direkt in der Konsole ausführen. Dies ist ein guter Weg, um mit R-Code zu experimentieren, denn Ihre Eingabe wird nicht auf Richtigkeit überprüft."
free_preview: true
---

## Wie R funktioniert

```yaml
type: NormalExercise
key: 2bafef99a3
lang: r
xp: 100
skills: 1
```

This is an example exercise.

`@instructions`
Im Editor auf der rechten Seite gibt es bereits einige Beispiel-Codes. Erkennen Sie, welche Linien tatsächlich die R Codes und welche Linien 	die Kommentare sind?
    Fügen Sie eine Codezeile hinzu, die die Summe von 6 und 12 berechnet und klicken Sie auf den Button "Antwort abschicken".

`@hint`
Fügen Sie eine Zeile R-Code ein, die die Summe von 6 und 12 berechnet, genau wie im Beispielcode demonstriert.

`@pre_exercise_code`
```{r}
6+12
```

`@sample_code`
```{r}

```

`@solution`
```{r}
6+12
```

`@sct`
```{r}
success_msg("Sehr gut")
```

---

## Starte mit R

```yaml
type: NormalExercise
key: 1e15c44df4
xp: 100
```

Erste Schritte, um R hands-on zu lernen und die interaktive Programmierumgebung kennenzulernen.

`@instructions`
Willkommen in der Programmierumgebung DataCamp. Lasst uns direkt loslegen. 

Hier Vorgeschichte Datenset + Problemstellung
Zurerst lese das zu bearbeitende Datenset "Verkaufsdaten" ein.

`@hint`
Nutze die Funktion #read.table() (liest externen Datensatz ein)

`@pre_exercise_code`
```{r}
library(dplyr)
read.table(https://assets.datacamp.com/production/repositories/4810/datasets/18ace2e3d5f4d3fa99765263c04573ba9bfae208/Verkaufsdaten_1.csv)
```

`@sample_code`
```{r}

```

`@solution`
```{r}
read.csv(Verkaufsdaten)
```

`@sct`
```{r}
success_msg("Nice work! Success messages are a great way to keep users engaged even after the exercise is over. Try to encourage them to play around in the console to really grasp the concepts you're trying to teach!")
```
