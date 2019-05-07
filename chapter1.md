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
6. Berechnen Sie 119 Modulo 13.
    
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
2
```

`@sct`
```{r}
codeaddition <- c("23+46", "23+46")
codesubtraktion <- c("234-64")
codemultiplikation <- c("222*59")
codedivision <- c("465/3")
codepotenzierung <- c("2^5", "2*2*2*2*2")
codemodulo <- c("119%%13", "119-9*13")
ex() %>% check_code(c(codeaddition, codesubtraktion, codemultiplikation, codedivision, codepotenzierung, codemodulo), fixed = TRUE)
success_msg("Gute Arbeit! Hast du richtig gut gemacht!")
```

---

## Rechnen mit R

```yaml
type: TabExercise
key: eb3ada4691
xp: 100
```

![Bier](https://assets.datacamp.com/production/repositories/4810/datasets/60bfcabd6718aeffbe70679de850ae528bf09cee/bier.jpg)

`@pre_exercise_code`
```{r}

```

***

```yaml
type: NormalExercise
key: f3ad798fa3
xp: 20
```

`@instructions`
Summieren Sie die Zahlen 23 und 46

`@hint`


`@sample_code`
```{r}
# Summieren Sie die Zahlen 23 und 46

```

`@solution`
```{r}

23+46
```

`@sct`
```{r}
codeaddition <- c("23+46", "23+46")
ex() %>% check_code(c(codeaddition), fixed = TRUE)
success_msg("Richtig, weiter geht es!")
```

***

```yaml
type: NormalExercise
key: dfd9aea716
xp: 20
```

`@instructions`
2. Ziehen Sie von der Zahl 2345 87 ab.

`@hint`


`@sample_code`
```{r}
# Ziehen Sie von der Zahl 2345 87 ab.

```

`@solution`
```{r}
2345-87
```

`@sct`
```{r}
codesubstraktion <- c("2345-87")
ex() %>% check_code(c(codesubstraktion), fixed = TRUE)
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: 33bebf536a
xp: 20
```

`@instructions`
Multiplizieren Sie die Zahlen 222 und 59

`@hint`


`@sample_code`
```{r}
# Multiplizieren Sie die Zahlen 222 und 59

```

`@solution`
```{r}
222*59
```

`@sct`
```{r}
codemultiplikation <- c("222*59", "59*222")
ex() %>% check_code(c(codemultiplikation), fixed = TRUE)
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: bfa213b421
xp: 20
```

`@instructions`
Potenzieren Sie 2 hoch 5

`@hint`


`@sample_code`
```{r}
# Potenzieren Sie 2 hoch 5

```

`@solution`
```{r}
2^5		
```

`@sct`
```{r}
codepotenzierung <- c("2^5", "2*2*2*2*2")
ex() %>% check_code(c(codepotenzierung), fixed = TRUE)
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: 94b44944a6
xp: 20
```

`@instructions`
Berechnen Sie 119 Modulo 13

`@hint`


`@sample_code`
```{r}
# Berechnen Sie 119 Modulo 13

```

`@solution`
```{r}
119 %% 13
```

`@sct`
```{r}
codemodulo <- c("119%%13", "2")
ex() %>% check_code(c(codemodulo), fixed = TRUE)
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: MultipleChoiceExercise
key: 6df8493e71
```

`@question`
Was ist das Ergebnis von 9 Modulo 2

`@possible_answers`
- [1]
- 2
- 3
- 9

`@hint`
Das geht im Kopf - hier geht es um Verständnis.

`@sct`
```{r}

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
Bsp.: Beachten Sie: Wenn Sie R nach x fragen, wird der Wert angezeigt.

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
ex() %>% check_object("x") %>% check_equal(42)
ex() %>% check_code(c("print(x)", "x"))
ex() %>% check_output("42", fixed=TRUE, missing_msg="So ist das nicht ganz richtig!")
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

- Natürliche Zahlen, wie 4, heißen auch ganze Zahlen ('Integers').
- Dezimalwerte, wie 4.5 werden auch Numerik ('Numerics') genannt.
- Boolesche Werte (TRUE oder FALSE) werden auch als Wahrheitswerte bezeichnet.
- Text-(oder String-)Werte werden als Zeichen ('Characters') benannt und Textwerte werden in "Anführungszeichen" gesetzt.

Bsp.: Der Variable x soll der Wert 25 zugewiesen werden: x <- 25.

`@instructions`
1. Geben Sie den Wert von my_numeric aus.
 
	Ändern Sie die Werte von:
 2. Variable my_numeric zu 13.
 3. Variable my_character zu "universe".
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
# Welchen Wert hat my_numeric:

# Weisen Sie my_numeric den Wert 54 zu:

# Verändern Sie my_character zu universe:

# Verändern Sie my_logical zu FALSE:

```

`@solution`
```{r}
# Geben Sie bitte den Wert von my_numeric aus:
print(my_numeric)
# Weisen Sie my_numeric den Wert:
my_numeric <- 54
# Verändern Sie my_character zu "universe":
my_character <- "universe"
# Verändern Sie my_logical zu FALSE:
my_logical <- FALSE
```

`@sct`
```{r}
ex() %>% check_code(c("print(my_numeric)", "my_numeric"), fixed = TRUE)
ex() %>% check_object("my_numeric")   %>% check_equal(54)
ex() %>% check_object("my_character") %>% check_equal("universe")
ex() %>% check_object("my_logical")   %>% check_equal("FALSE")
success_msg("Ja, genau - es sieht so aus als hätten Sie die Variablenzuweisung verstanden!")
```

---

## Erstellen eines Vektors

```yaml
type: NormalExercise
key: bd8c85316c
xp: 100
```

Vektoren erzeugen und erstellen:
- Ein Vektor ist die einfachste Datenstruktur in R und wird als "einzelnes Objekt, das aus einer Ansammlung von Dingen besteht" definiert (R-Handbuch). Es ist die kleinstmögliche Dateneinheit in R. (de Vries/Meys 2018)
Bsp.: Um einen Vektor mit den Zahlen von 1 bis 2 zu erzeugen: myfirstvector <- c(1,2).

`@instructions`
1. Erstellen Sie einen Vektor mit dem Namen my_vec, der die Zahlen von 1 bis 5 beinhaltet.
2. Berechnen Sie den Durchschnitt (mean) des Vektors my_vec und weisen Sie ihm dem Namen my_mean zu.

`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# 1. Erstellen Sie einen Vektor mit dem Namen my_vec, der die Zahlen von 1 bis 5 beinhaltet.

# 2. Berechnen Sie den Durchschnitt (mean) des Vektors my_vec und weisen Sie ihm dem Namen my_mean zu.

```

`@solution`
```{r}
# 1. Erstellen Sie einen Vektor mit dem Namen my_vec, der die Zahlen von 1 bis 5 beinhaltet:
my_vec <- c(1,2,3,4,5)

# 2. Berechnen Sie den Durchschnitt (mean) des Vektors my_vec und weisen Sie ihm dem Namen my_mean zu.
my_mean <- mean(my_vec)
```

`@sct`
```{r}
ex() %>% check_object("my_vec") %>% check_equal("c(1,2,3,4,5)", "c(1:5)")
ex() %>% check_object("my_mean") %>% check_equal("mean(my_vec)")
ex() %>% check_object("my_mean") %>% check_equal(3)
success_msg("Ja, genau - es sieht so aus als hätten Sie die Variablenzuweisung verstanden!")
```

---

## (Matrizen)

```yaml
type: NormalExercise
key: 3e48f500af
xp: 100
```

Matrizen sind eine rechteckige Anordnung (Tabelle) von Elementen. In R können komplexe Matrixoperationen einfach und effizient durchgeführt werden. In der Statistik werden häufig Matrixberechnungen angewandt. (de Vries/Meys 2018)

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

Bislang war immer von einem Vektor die Rede. Des Weiteren gibt es noch Matrizen, die wir aufgrund der Kürze der Einführung in diesem Kurs überspringen.

Nun kommen wir direkt zu den **Data Frames**:
In eine Matrix bekommen Sie diese Daten unterschiedlichen Datentyps nur, wenn Sie alles in Text umwandeln, was jedoch die Auswertung erschwert. Deswegen wird ein Data Frame verwendet, da Sie in diesem alle Daten unterschiedlichen Typs speichern können. Dieses Objekt (Tabelle) heißt in R Data Frame. (Quelle: De Vries/Meys 2018, S.146)

Der Datensatz des Unternehmens Bambergus, der aus der zentralen Kundendatenbank stammt, enthält verschiedene Kundeninformationen.
Welche Rubriken sind dies? Denken Sie an die Ausgabe. Der Name des Datensatzes trägt den Namen # Kundendaten und ist eine Variable. der Verkaufsgegenstände, den jeweiligen Preis, die Absatzmenge pro Quartal, für welche Kundenart er verkauft wurde.

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

---

## Insert exercise title here

```yaml
type: TabExercise
key: 147d6f2f44
xp: 100
```



`@pre_exercise_code`
```{r}

```
