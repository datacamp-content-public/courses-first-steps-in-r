---
title: 'Wie R funktioniert'
description: "Um die Übung zu lösen, geben Sie im Editor auf der rechten Seite den R-Code ein. Wenn Sie auf den Button \"Submit Answer\" klicken, wird jede Codezeile interpretiert und durch R ausgeführt. Sie erhalten eine Nachricht, ob der von Ihnen erstellte Code richtig war. Ihre Ausgabe des R-Codes wird in der Konsole unten rechts angezeigt.\n\nIn R wird die #-Taste genutzt, um Kommentare zu kennzeichnen, die Ihnen und anderen R-Nutzern zusätzliche Informationen über den Code bereitstellen. Kommentare werden nicht als R-Code ausgeführt, somit beeinflussen sie die Ergebnisse nicht. Zum Beispiel Berechnen Sie 3+4 ist im Editor rechts ein Kommentar.\n\nSie können die R-Befehle auch direkt in der Konsole ausführen. Dies ist ein guter Weg, um mit R-Code zu experimentieren, denn Ihre Eingabe wird nicht auf Richtigkeit überprüft."
free_preview: true
---

## Motivation | Einstieg | Was  ist Data Science

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
- Im Editor auf der rechten Seite gibt es bereits einige Beispiel-Codes. Beachten Sie, dass es Unterschiede in den Zeilen gibt - sie beinhalten Code und mit dem '#' werden Kommentare gekennzeichnet.
- Fügen Sie bitte zuerst eine Codezeile hinzu, die die Summe von 14 und 32 berechnet und klicken Sie danach auf "Submit Answer" (Antwort abschicken).

`@hint`
1. Fügen Sie bitte eine Zeile R-Code ein, die die Summe von 67 und 78 berechnet, genau wie im Beispielcode demonstriert.
2. Stellen Sie sicher, dass Sie '14 + 32' in einer neuen Zeile eingefügt haben. Starten Sie die Zeile nicht mit einem '#'-Zeichen, ansonsten wird der geschriebene Code nicht wie gewünscht ausgeführt, da damit Kommentare gekennzeichnet werden!

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Addition 67+78
67+78
# Ihre Lösung für die zweite Addition

```

`@solution`
```{r}
67+78

14+32
```

`@sct`
```{r}
codeaddition <- c("14+32", "32+14")
ex() %>% check_code(c(codeaddition), fixed = TRUE)
success_msg("Sie sehen das Ergebnis in der Console. Sehr gut gemacht.")
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

	Der Potenzierungs-Operator (^) steigert die linke Zahl durch die Größe der rechten Zahl: Zum Beispiel 4^2 ist 16.
    Der Operator Modulo (%%) liefert den Rest durch die Division der linken Zahl durch die rechte Zahl, zum Beispiel 7 %% 2 ist 1.

Behalten Sie diese Informationen im Hinterkopf und befolgen Sie sie in den nachstehenden Aufgaben, um die Übung erfolgreich abzuschließen.

`@instructions`
1. Summieren Sie die Zahlen 23 46
2. Ziehen Sie von der Zahl 234 64 ab.
3. Multiplizieren Sie die Zahlen 222 und 59
4. Dividieren Sie 465 durch 3
5. Potenzieren Sie 2 hoch 5
6. Berechnen Sie 28 Modulo 6.
    
Klicken Sie nach dem Programmieren auf 'Submit Answer' und schauen Sie sich die R-Ausgabe in der Konsole an. 
Beachten Sie, wie das '#' Symbol in den R-Codes verwendet wird.

`@hint`
1. Achten Sie bitte auf die richtigen Operatoren und mögliche Tippfehler, da diese als Fehler ausgegeben werden.
2. Ein weiteres Beispiel für den Modulo Operator ist: 9 %% 2 gleich 1.

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
13098
#4 Division
155
#5 Potenzierung
32
#6 Modulo
4
```

`@sct`
```{r}
codeaddition <- c("23+46", "23+46")
codesubtraktion <- c("234-64")
codemultiplikation <- c("222*59")
ex() %>% check_code(c(codeaddition, codesubtraktion, codemultiplikation), fixed = TRUE)
success_msg("Gute Arbeit! Hast du richtig gut gemacht!")
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

Eine Variable ermöglicht es einen Wert (z.B. 4) oder ein Objekt (z.B. Funktionsbeschreibung) in R zu speichern. Später können Sie den Namen der Variable nutzen, um einfach auf den Wert oder das Objekt zuzugreifen, die innerhalb dieser Variablen hinterlegt sind.

So können Sie der Variable my_var den Wert 4 zuweisen: my_var <- 4

`@instructions`
Ihre Aufgabe: 
Vervollständigen Sie bitte den Code im Editor, sodass der Variable x der Wert 42 zugeordnet wird. Schicken Sie dann die Antwort ab. 
Beachten Sie: Wenn Sie R nach x fragen, wird der Wert angezeigt.

`@hint`
Der Variable my_var wurde jetzt im Beispiel der Wert 4 zugeteilt. Orientieren Sie sich einfach daran.

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
zuweisung <- c("x <- 42")
ausgabe <- c("print(x)", "x")
ex() %>% check_code(c(zuweisung, ausgabe), fixed = TRUE)
success_msg("Ja, genau - es sieht so aus als hätten Sie die Variablenzuweisung verstanden!")
```

---

## Basisdatentypen in R

```yaml
type: NormalExercise
key: bd7572143c
xp: 100
```

R arbeitet mit zahlreichen Datentypen und ist sensitiv auf Groß-/Kleinschreibung. Einige der grundlegendsten Datentypen sind:
```
Natürliche Zahlen, wie 4, heißen auch ganze Zahlen ('Integers').
Dezimalwerte, wie 4.5 werden auch Numerik ('Numerics') genannt.
Boolesche Werte (TRUE oder FALSE) werden auch als 'logicals' bezeichnet.
Text-(oder String-)Werte werden als Zeichen ('characters') benannt und Texte werden in "Anführungszeichen" gesetzt.
```
Bsp.: Der Variable x soll der Wert 25 zugewiesen werden: x <- 25.

`@instructions`
1. Geben Sie den Wert von my_numeric aus.
 
Ändern Sie die Werte von:
 2. Variable my_numeric zu 13.
 3. Variable my_character zu "universe". Beachten Sie den Datentyp.
 4. Variable my_logical zu FALSE.

`@hint`
```
1. Kommen Sie, einfach die Variable reinschreiben oder mit dem Operator print(Variable) ausgeben lassen.
```
```
2. Ersetzen Sie die Werte im Editor mit den Werten, die bei der Anweisung vorgegeben sind. 
Zum Beispiel: my_numeric <- 13 , um der Variable my_numeric den Wert 13 zuzuweisen.
```

`@pre_exercise_code`
```{r}
my_numeric <- 3
```

`@sample_code`
```{r}
# Welchen Wert hat my_numeric

# Verändern Sie my_numeric zu 54

# Verändern Sie my_character zu "universe"

# Verändern Sie my_logical zu FALSE

```

`@solution`
```{r}
# Welchen Wert hat my_numeric
print(my_numeric)
# Verändern Sie my_numeric zu 42
my_numeric <- 54
# Verändern Sie my_character zu "universe"
my_character <- "universe"
# Verändern Sie my_logical zu FALSE
my_logical <- FALSE
```

`@sct`
```{r}
codewert <- c(print(my_numeric), "my_numeric")
codezuweisung <- c("my_numeric <- 54")
character <- c("my_character <- universe")
boolean <- c("my_logical <- FALSE")
ex() %>% check_code(c(codewert, codezuweisung, character, boolean), fixed = TRUE)
success_msg("Gute Arbeit - so langsam werden Sie warm ;)!", praise = FALSE)
```

---

## Erstellen eines Vektors

```yaml
type: NormalExercise
key: bd8c85316c
xp: 100
```

Hier Beschreibung von Vektoren und Sinnhaftigkeit!

`@instructions`
1. Erstellen Sie einen Vektor mit dem Namen my_vec, der die Zahlen von 1 bis 5 beinhaltet.
2. Berechnen Sie den Durchnitt (mean) des Vektors my_vec und weisen Sie ihm dem Namen my_mean zu.

`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Erstellen Sie einen Vektor, der die Zahlen von 1 bis 5 beinhaltet.

# Berechnen Sie den Durchnitt (arithmetisches Mittel) von dem vorher angelegten Vektor. Beachten Sie, der Code ist immer im Englischen zu schreiben.

```

`@solution`
```{r}
# Erstellen Sie einen Vektor, der die Zahlen von 1 bis 5 beinhaltet.
my_vec <- c(1,2,3,4,5)

# Berechnen Sie den Durschnnitt von dem vorher angelegten Vektor.
my_mean <- mean(my_vec)
```

`@sct`
```{r}
vector <- c("my_vec <- c(1,2,3,4,5)", "my_vec <- c(1:5)")
mean <- c("my_mean <- mean(my_vec)")
ex() %>% check_code(c(vector, mean), fixed = TRUE)
success_msg("Top. Gut programmiert", praise = FALSE)
```

---

## (Matrizen)

```yaml
type: NormalExercise
key: 3e48f500af
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

## Data Frames

```yaml
type: NormalExercise
key: 35f2e90e22
xp: 100
```

Bislang war immer von einem Vektor die Rede. Des Weiteren gibt es noch Matrizen, die wir aufgrund der Kürze der Einführung in diesem Kurs überspringen. Nun kommen wir direkt zu den Data Frames

**Data Frames:**
Der Datensatz des folgenden Unternehmens der aus der Datenbank des Informationssystem stammt, enthält den Namen der Verkaufsgegenstände, den jeweiligen Preis, die Absatzmenge pro Quartal, für welche Kundenart er verkauft wurde. In eine Matrix bekommen Sie diese Daten nur, wenn Sie alles in Text umwandeln, was jedoch die Auswertung erschwert. Deswegen wird ein Data Frame verwendet, da Sie in diesem alle Daten unterschiedlichen Typs speichern können. Dieses Objekt heißt in R (data frame). 
(Quelle: De Vries/Meys 2018, S.146)

`@instructions`


`@hint`


`@pre_exercise_code`
```{r}
Kundendaten <- read.csv2("https://assets.datacamp.com/production/repositories/4810/datasets/31e25bf7206a508aa8681c19698e57afc52ab492/dataMay-3-2019.csv")
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
