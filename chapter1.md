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

Lasst uns mit der ersten Aufgabe starten! Let´s go!

`@instructions`
- Im Editor auf der rechten Seite gibt es bereits einige Beispiel-Codes. Erkennen Sie, welche Linien tatsächlich die R Codes und welche Linien 	die Kommentare sind?
- Fügen Sie eine Codezeile hinzu, die die Summe von 6 und 12 berechnet und klicken Sie auf den Button "Antwort abschicken".

`@hint`
1. Fügen Sie eine Zeile R-Code ein, die die Summe von 6 und 12 berechnet, genau wie im Beispielcode demonstriert.
2. Stellen Sie sicher, dass Sie '6 + 12' in einer neuen Zeile eingefügt haben. Starten Sie die Zeile nicht mit einem '#'-Zeichen, ansonsten wird Ihr Code nicht ausgeführt!!

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
6+12
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

## Rechnen mit R

```yaml
type: NormalExercise
key: 729f60ecbd
xp: 100
```

Rechnen mit R:
In seiner grundlegendsten Form kann R als ein einfacher Rechner verwendet werden. Beachten Sie folgende Rechenoperatoren:

	Addition: +
    Subtraktion: -
    Multiplikation: *
    Division: /
    Potenzierung: ^
    Modulo: %%

Die letzten beiden Operatoren benötigen eine Erklärung:

    Der ^ Operator steigert die linke Zahl durch die Größe der rechten Zahl, es ist die Potenz: Zum Beispiel 3^2 ist 9.

    Der Operator Modulo liefert den Rest durch die Division der linken Zahl durch die rechte Zahl, zum Beispiel 5 Modulo 3 oder 5 %% 3 ist 2.

Behalten Sie diese Informationen im Hinterkopf und befolgen Sie die nachstehenden Anweisungen, um die Übung abzuschließen.

`@instructions`
1. Summieren Sie die Zahlen 23 46
 2. Ziehen Sie von der Zahl 234 64 ab.
 3. Multiplizieren Sie die Zahlen 222 und 59
 4. Dividieren Sie 465 durch 3
 5. Potenzieren Sie 2 hoch 5
 6. Berechnen Sie 28 Modulo 6.
    
Klicken Sie auf 'Antwort abschicken' und schauen Sie sich die R-Ausgabe in der Konsole an. 
Beachten Sie, wie das '#' Symbol in den R-Codes verwendet wird. (Damit sind Kommentare gekennzeichnet.)

`@hint`
Ein weiteres Beispiel für den Modulo Operator: 9 %% 2 gleich 1.

`@pre_exercise_code`
```{r}
#1 Addition

#2 Subtraktion

#3 Multiplikation

#4 Division

#5 Potenzierung

#6 Modulo

```

`@sample_code`
```{r}
#1 Addition

#2 Subtraktion

#3 Multiplikation

#4 Division

#5 Potenzierung

#6 Modulo
```

`@solution`
```{r}
#1 Addition
69
#2 Subtraktion
170
#3 Multiplikation
222
#4 Division
13098
#5 Potenzierung
32
#6 Modulo
4
```

`@sct`
```{r}
success_msg("Nice work! Hast du richtig gut gemacht!")
```

---

## Variablenzuweisung

```yaml
type: NormalExercise
key: b16f728974
xp: 100
```

Variablenzuweisung

Ein grundlegendes Konzept in der (statistischen) Programmierung sind Variablen.

Eine Variable ermöglicht es Ihnen, einen Wert (z.B. 4) oder ein Objekt (z.B. Funktionsbeschreibung) in R zu speichern. Später können Sie den Namen der Variable nutzen, um einfach auf den Wert oder das Objekt zuzugreifen, die innerhalb dieser Variable hinterlegt sind.

Sie können der Variable my_var den Wert 4 zuweisen.

my_var <- 4

`@instructions`
Ihre Aufgabe: Vervollständigen Sie den Code im Editor, sodass der Variable x der Wert 42 zugeordnet wird. Schicken Sie Ihre Antwort ab. Beachten Sie: Wenn Sie R nach x fragen, wird der Wert 42 angezeigt.

`@hint`
Der Variable my_var wurde jetzt im Beispiel der Wert 4 zugeteilt. Machen Sie genau das Gleiche im Editor, aber statt dem Wert 4 ordnen Sie der Variable x den Wert 42 zu.

`@pre_exercise_code`
```{r}


```

`@sample_code`
```{r}
# Weisen Sie x den Wert 42 zu

# Geben Sie den Wert der Variable x aus
```

`@solution`
```{r}
# Weisen Sie x den Wert 42 zu
x <- 42
# Geben Sie den Wert der Variable x aus
x
```

`@sct`
```{r}

```

---

## Hands-on R: Lasst uns anfangen

```yaml
type: NormalExercise
key: 1e15c44df4
xp: 100
```

Erste Schritte, um R 'hands-on' zu lernen und die interaktive Programmierumgebung kennenzulernen.
Hier sehen Sie den Data Science Zyklus. Diesen werden wir Schritt für Schritt anhand eines Teaching Cases durchgehen.
![1](https://assets.datacamp.com/production/repositories/4810/datasets/82d92f41d7649657073e1e2e0b813011ecc4973a/Data_Science_Explore.png)

`@instructions`
Willkommen in der Programmierumgebung DataCamp. Lasst uns nun direkt mit dem Datensatz loslegen. 

Hier Vorgeschichte Datenset + Problemstellung + Was macht ein DataScientist
Zuerst lese das zu bearbeitende Datenset "Verkaufsdaten" ein.!

`@hint`
Nutze die Funktion #read.table() 
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
success_msg("Nice work! Success messages are a great way to keep users engaged even after the exercise is over. Try to encourage them to play around in the console to really grasp the concepts you're trying to teach!")
```
