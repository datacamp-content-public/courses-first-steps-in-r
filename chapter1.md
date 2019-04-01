---
title: 'Wie R funktioniert'
description: "Um die Übung zu lösen, geben Sie im Editor auf der rechten Seite den R-Code ein. Wenn Sie auf den Button \"Submit Answer\" klicken, wird jede Codezeile interpretiert und durch R ausgeführt. Sie erhalten eine Nachricht, ob der von Ihnen erstellte Code richtig war. Ihre Ausgabe des R-Codes wird in der Konsole unten rechts angezeigt.\n\nIn R wird die #-Taste genutzt, um Kommentare zu kennzeichnen, die Ihnen und anderen R-Nutzern zusätzliche Informationen über den Code bereitstellen. Kommentare werden nicht als R-Code ausgeführt, somit beeinflussen sie die Ergebnisse nicht. Zum Beispiel Berechnen Sie 3+4 ist im Editor rechts ein Kommentar.\n\nSie können die R-Befehle auch direkt in der Konsole ausführen. Dies ist ein guter Weg, um mit R-Code zu experimentieren, denn Ihre Eingabe wird nicht auf Richtigkeit überprüft."
free_preview: true
---

## Motivation | Einstieg

```yaml
type: VideoExercise
key: 643e42346b
xp: 50
```

`@projector_key`
9ef46453f6f5df6af0792122ac091c86

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

    Der ^ Operator steigert die linke Zahl durch die Größe der rechten Zahl, es ist die Potenz: Zum Beispiel 4^2 ist 16.
    Der Operator Modulo liefert den Rest durch die Division der linken Zahl durch die rechte Zahl, zum Beispiel 7 Modulo 2 oder 7 %% 2 ist 1.

Behalten Sie diese Informationen im Hinterkopf und befolgen Sie die nachstehenden Anweisungen, um die Übung abzuschließen.

`@instructions`
1. Summieren Sie die Zahlen 23 46
2. Ziehen Sie von der Zahl 234 64 ab.
3. Multiplizieren Sie die Zahlen 222 und 59
4. Dividieren Sie 465 durch 3
5. Potenzieren Sie 2 hoch 5
6. Berechnen Sie 28 Modulo 6.
    
Klicken Sie auf 'Submit Answer' und schauen Sie sich die R-Ausgabe in der Konsole an. 
Beachten Sie, wie das '#' Symbol in den R-Codes verwendet wird. (Damit sind Kommentare gekennzeichnet.)

`@hint`
Ein weiteres Beispiel für den Modulo Operator ist: 9 %% 2 gleich 1.

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

## Test für das Abfangen der Fehllösungen

```yaml
type: NormalExercise
key: 79b661d576
xp: 100
```



`@instructions`
5 + 12

`@hint`
Auf geht´s - nimm es leicht, einfach eintippen, wie im eigenen Taschenrechner

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Rechnung hier eintragen
```

`@solution`
```{r}
17
```

`@sct`
```{r}
ex() %>% check_code(c("5+12", "12+5"), fixed = TRUE)
success_msg("Super!", praise = FALSE)
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

Eine Variable ermöglicht es Ihnen, einen Wert (z.B. 4) oder ein Objekt (z.B. Funktionsbeschreibung) in R zu speichern. Später können Sie den Namen der Variable nutzen, um einfach auf den Wert oder das Objekt zuzugreifen, die innerhalb dieser Variablen hinterlegt sind.

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

## Basisdatentypen in R

```yaml
type: NormalExercise
key: bd7572143c
xp: 100
```

Basisdatentypen in R

   R arbeitet mit zahlreichen Datentypen. Einige der grundlegendsten Datentypen sind:
   
   Dezimalwerte, wie 4.5 werden auch 'numerics' (Numerik) genannt.
   Natürliche Zahlen, wie 4, heißen auch 'integers' (Ganze Zahlen). Ganze Zahlen sind auch Numerik.
   Boolesche Werte (TRUE oder FALSE) werden auch 'logical' (logisch) genannt.
   Text- (oder String-) Werte werden auch als 'characters' (Zeichen) bezeichnet.
   
Beachten Sie, wie die Anführungszeichen auf der rechten Seite zeigen, dass "einige Texte" ein Zeichen sind.

`@instructions`
Ändern Sie die Werte von:

 1. Variable my_numeric zu 13.
 2. Variable my_character zu "universe". Beachten Sie, dass die Anführungszeichen zeigen, 
 	dass "universe" ein Zeichen ist.
 3. Variable my_logical zu FALSE.
    
Beachten Sie in R die Groß- und Kleinschreibung.

`@hint`
Ersetzen Sie die Werte im Editor mit den Werten, die bei der Übung vorgesehen sind. 
Zum Beispiel: my_numeric <- 13 , um der Variable my_numeric den Wert 13 zuzuweisen.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Verändern Sie my_numeric zu 42

# Verändern Sie my_character zu "universe"

# Verändern Sie my_logical zu FALSE

```

`@solution`
```{r}

```

`@sct`
```{r}

```

---

## Erstelle einen Vektors

```yaml
type: NormalExercise
key: bd8c85316c
xp: 100
```



`@instructions`
1. Create a vector called my_vect containing 1 through 5.
2. Take the mean of my_vect and assign it to a variable named my_mean. Use the mean() function.
3. Use my_mean to compute the sum of squares of my_vect. Use the sum() function.

`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Create a vector called my_vect containing 1 through 5

# Take the mean and assign to my_mean

# Use my_mean to compute the sum of squares of my_vect

```

`@solution`
```{r}
# Create a vector called my_vect containing 1 through 5
my_vect <- c(1,2,3,4,5)

# Take the mean and assign to my_mean
my_mean <- mean(my_vect)

# Use my_mean to compute the sum of squares of my_vect
sum((my_vect - my_mean)^2)
```

`@sct`
```{r}
success_msg("Wunderbar", praise = FALSE)
```

---

## Matrix 

```yaml
type: NormalExercise
key: 3e48f500af
xp: 100
```

ggf. Matrix hier einfügen

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

## Data Frames

```yaml
type: NormalExercise
key: 35f2e90e22
xp: 100
```

Bislang war immer von ein Vektor die Rede. Des Weiteren gibt es noch Matrizen, die wir aufgrund der Einführung in diesem Kurs weglassen werden.

**Data Frames:**
Der Datensatz des folgenden Unternehmens der aus der Datenbank des Informationssystem stammt, enthält den Namen der Verkaufsgegenstände, den jeweiligen Preis, die Absatzmenge pro Quartal, für welche Kundenart er verkauft wurde. In eine Matrix bekommen Sie diese Daten nur, wenn Sie alles in Text umwandeln, was jedoch die Auswertung erschwert. Deswegen wird ein Data Frame verwendet, da Sie in diesem alle Daten unterschiedlichen Typs speichern können. Dieses Objekt heißt in R (data frame). 

(ggf. noch ändern: de Vries/Meys 2018, S.146)

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

## Haben Sie es verstanden?

```yaml
type: PureMultipleChoiceExercise
key: a24e1b005a
xp: 50
```

14 %% 3

`@hint`


`@possible_answers`
- 5
- 4
- 3
- [2]
- 1

`@feedback`
- "Nein, da haben Sie etwas falsch verstanden"
- "Nein, da liegen Sie nicht richtig"
- "Nein, da liegen Sie nicht richtig"
- "Super gemacht, 14 Modulo 3 ergibt 2"
- "Nein, da liegen Sie nicht richtig"
