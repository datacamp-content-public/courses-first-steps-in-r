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

## Wie R in Data Camp funktioniert

```yaml
type: NormalExercise
key: 2bafef99a3
lang: r
xp: 100
skills: 1
```

Lasst uns mit der ersten Aufgabe starten! Let´s go!

`@instructions`
Hallo und herzlich Willkommen,

Sie sind unser/e neue/r MitarbeiterIn in der IT-Abteilung und befassen sich das erste Mal mit der Programmiersprache R. Ihr Chef Herr Müller hat Ihnen verschiedene Aufgaben gegeben, nun fangen wir aber erstmal leicht an. 

![](https://assets.datacamp.com/production/repositories/4810/datasets/44f5b387423e2b1a9a47c24d837c1bd4f3184ee0/IT_Mitarbeiter.jpg)

- Wir fangen mit dem Programm an, mit dem auch viele Programmierbücher starten: "Hello World!"
	- Dafür schreiben Sie bitte: **print("Hello World!")** in das Skript und drücken auf 'Submit Answer'

`@hint`
Keine Angst - einfach print("Hello World!") in das Script schreiben und auf 'Submit Answer' drücken.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Ihr erstes Programm: "Hello World!"

```

`@solution`
```{r}
# Erstes Programm: "Hello World!"
print("Hello World!")
```

`@sct`
```{r}
ex() %>% check_output("Hello World!", fixed=TRUE, missing_msg= "So ist das nicht ganz richtig - Beachten Sie Tippfehler!")
success_msg("So ihr erstes Programm ist vollendet! ![Welt](https://assets.datacamp.com/production/repositories/4810/datasets/efdb2635ca5a59a67d67dedea62813ca4cf68a0d/hello_welt.jpg)")
```

---

## Rechnen mit R

```yaml
type: TabExercise
key: eb3ada4691
xp: 100
```

In seiner grundlegendsten Form kann R als ein einfacher Rechner verwendet werden. Beachten Sie folgende Rechenoperatoren:	 
```
 - Addition: + 
 - Subtraktion: - 
 - Multiplikation: * 
 - Division: / 
 - Potenzierung: ^ (z.B. 4^2 ist 16)
 - Modulo: %% 
```
Der Operator Modulo (%%) liefert den Rest der Division der linken Zahl durch die rechte Zahl: z.B.: 7 %% 2 ist 1.

Behalten Sie diese Informationen im Hinterkopf und befolgen Sie sie in den nachfolgenden Aufgaben, um die Übung erfolgreich abzuschließen.

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
- Im Editor auf der rechten Seite gibt es bereits einige Beispiel-Codes. Beachten Sie, dass es Unterschiede in den Zeilen gibt - sie beinhalten Code und mit dem **'#'** werden Kommentare gekennzeichnet.
- Sie sollen die Umsätze der letzten drei Monate zusammenrechnen und somit den Umsatz für das Quartal Q1 erstellen. Fügen Sie bitte eine weitere Codezeile hinzu, fügen Sie Ihre Rechnung ein und klicken Sie danach auf "Submit Answer". Schauen Sie anschließend bitte in die Console.

```
Umsatz: Jannuar 23400 | Februar 32000 | März 29400
```

`@hint`
Stellen Sie sicher, dass Sie die Summe aus 234000 + 320000 + 294000 in einer neuen Zeile eingefügt haben. Starten Sie die Zeile nicht mit einem '#'-Zeichen, ansonsten wird der geschriebene Code nicht wie gewünscht ausgeführt, da damit Kommentare gekennzeichnet werden!

`@sample_code`
```{r}
# Beispielcode Addition 
67+78
# Ihre eigene Berechnung:

```

`@solution`
```{r}
# Beispielcode Addition 
67+78
# Ihre eigene Berechnung:
234000 + 320000 + 294000
```

`@sct`
```{r}
ex() %>% check_output(145, fixed=TRUE, missing_msg= "So ist das nicht richtig - beachten Sie Tippfehler!")
ex() %>% check_output(848000, fixed=TRUE, missing_msg= "So ist das nicht ganz richtig - beachten Sie Tippfehler!")
success_msg("Ja, genau - der Umsatz im ersten Quartal beträgt 848.000€!")
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
ex() %>% check_output(2258, fixed=TRUE, missing_msg="So ist das nicht richtig - beachten Sie Tippfehler!")
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: 33bebf536a
xp: 20
```

`@instructions`
3. Multiplizieren Sie die Zahlen 222 und 59

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
ex() %>% check_output(13098, fixed=TRUE, missing_msg="So ist das nicht ganz richtig - beachten Sie Tippfehler!")
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: bfa213b421
xp: 20
```

`@instructions`
4. Potenzieren Sie 2 hoch 5

`@hint`
Haben Sie den Potenzierungsoperator ^ korrekt eingegeben? Schauen Sie nochmal konkret auf Ihre Berechnung.

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
ex() %>% check_output(32, fixed=TRUE, missing_msg="Nicht ganz richtig - beachten Sie Tippfehler!")
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: 94b44944a6
xp: 20
```

`@instructions`
5. Berechnen Sie 119 Modulo 13

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
ex() %>% check_output(2, fixed=TRUE, missing_msg="So ist das nicht ganz richtig - beachten Sie Tippfehler!")
success_msg("Richtig")
```

***

```yaml
type: MultipleChoiceExercise
key: 6df8493e71
```

`@question`
Wie lautet das Ergebnis von 10 Modulo 4

`@possible_answers`
- 1
- [2]
- 3
- 9

`@hint`
Das geht im Kopf - hier geht es nun um das Verständnis. Sie können aber auch die Console in R verwenden.

`@sct`
```{r}
ex() %>% check_code(-[2], fixed=TRUE, missing_msg="Leider nicht richtig, überlegen Sie noch einmal!")
success_msg("Richtig")
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
Wenn Sie R nach x fragen, wird der vorher zu gewiesene Wert angezeigt.

`@hint`
Der Variable my_var wurde im Beispiel der Wert 4 zugeteilt. Orientieren Sie sich einfach an dieser Vorgehensweise.

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
- Texte-(oder String-)werte werden als Zeichen ('Characters') benannt. **Wichtig:** Zeichenketten werden in "Anführungszeichen" gesetzt.

Bsp.: Der Variable x soll der Wert 25 zugewiesen werden: x <- 25.

`@instructions`
1. Geben Sie den Wert von my_nummerus aus.
 
	Ändern Sie die Werte von:
 2. Variable my_numeric zu 13.
 3. Variable my_character zu der Zeichenkette universe.
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
my_nummerus <- 3
```

`@sample_code`
```{r}
# Welchen Wert hat my_nummerus:

# Weisen Sie my_numeric den Wert 54 zu:

# Verändern Sie my_character zu der Zeichenkette universe:

# Verändern Sie my_logical zu FALSE:

```

`@solution`
```{r}
# Geben Sie bitte den Wert von my_nummerus aus:
print(my_nummerus)
# Weisen Sie my_numeric den Wert:
my_numeric <- 54
# Verändern Sie my_character zu  der Zeichenkette universe:
my_character <- "universe"
# Verändern Sie my_logical zu FALSE:
my_logical <- FALSE
```

`@sct`
```{r}
ex() %>% check_code(c("print(my_nummerus)", "my_nummerus"), fixed = TRUE)
ex() %>% check_output("3", fixed=TRUE, missing_msg="Da stimmt etwas nicht!")
ex() %>% check_object("my_numeric")   %>% check_equal(54)
ex() %>% check_object("my_character") %>% check_equal("universe")
ex() %>% check_object("my_logical")   %>% check_equal("FALSE")
success_msg("Ja, genau - es sieht so aus als hätten Sie die Basisdatentypen verstanden!")
```

---

## Vektoren

```yaml
type: TabExercise
key: 2a988ba927
xp: 100
```

Ein Vektor ist die einfachste Datenstruktur in R. Als "einzelnes Objekt, das aus einer Ansammlung von Dingen besteht" wird ein Vektor im R-Handbuch definiert. Es ist die kleinstmögliche Dateneinheit in R (de Vries/Meys 2018). Wir behandeln in dieser Einheit zum Einstieg nur numerische Vektoren, also Vektoren, die alle Arten von Zahlen enthalten können.

Vektoren erzeugen: 

Um einen Vektor mit einer Folge von Zahlen von 1 bis 3 zu erzeugen:  **c(1,2,3) oder kürzer c(1:3)**

Typ eines Vektors bestimmen und Überblick verschaffen: **str()**

Durchschnitt ausrechnen: **mean()**

`@pre_exercise_code`
```{r}
sell.time <- c(8,8,8,8,9,6)
```

***

```yaml
type: NormalExercise
key: ddc67f62d4
xp: 25
```

`@instructions`
1. Erstellen Sie einen Vektor, der die Zahlen von 1 bis 6 beinhaltet und weisen Sie ihm bitte den Namen open.vec zu. Die Zahlen stehen jeweils für einen Verkaufstag (1= Montag)

`@hint`
Schauen Sie bitte in die Erläuterungen, dort sind Beispiele gegeben.

`@sample_code`
```{r}
# Verkaufstage

```

`@solution`
```{r}

open.vec <- c(1:6)
```

`@sct`
```{r}
ex() %>% check_object("open.vec") %>% check_equal("c(1,2,3,4,5,6)", "c(1:6)", fixed=TRUE, missing_msg="So ist das nicht ganz richtig!")
success_msg("Ja, genau!")
```

***

```yaml
type: NormalExercise
key: a78b313e8c
xp: 25
```

`@instructions`
2. In dem Vektor sell.time ist die Verkaufszeit für jeden Verkaufstag hinterlegt. Lassen Sie sich bitte die Informationen über Typ und Struktur des Vektors sell.time ausgeben. Beurteilen Sie bitte, ob dieser nur numerische Zahlen enthält und welcher Tag der zeitlich Längste ist.

`@hint`
Die Funktion str() haben Sie in der Kontextbeschreibung gegeben.

`@sample_code`
```{r}
#Verkaufszeit

```

`@solution`
```{r}

str(sell.time)
```

`@sct`
```{r}
ex() %>% check_object("str(sell.time)", fixed=TRUE, missing_msg="Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau!")
```

***

```yaml
type: NormalExercise
key: fb1812faa3
xp: 25
```

`@instructions`
3. Am Freitag wurden 5103 Euro Umsatz generiert. Wie viel wurde pro Stunde umgesetzt?

`@hint`


`@sample_code`
```{r}
# Umsatz pro Stunde am Freitag:

```

`@solution`
```{r}

5103/9
```

`@sct`
```{r}
ex() %>% check_output(567, fixed=TRUE, missing_msg="Nicht richtig, da haben Sie sich wahrscheinlich verrechnet!")
success_msg("Richtig. Am Freitag wurden 567 Euro Umsatz pro Stunde erwirtschaftet!")
```

***

```yaml
type: NormalExercise
key: 05a1752bca
xp: 25
```

`@instructions`
4. Berechnen Sie bitte die tägliche durchschnittliche Verkaufszeit pro Verkaufstag.

`@hint`


`@sample_code`
```{r}
# Durchschnittliche Verkaufszeit:

```

`@solution`
```{r}

mean(sell.time)
```

`@sct`
```{r}
ex() %>% check_output(46/6, fixed=TRUE, missing_msg="Nicht ganz richtig - beachten Sie Tippfehler!")
success_msg("Richtig - die durschnittliche tägliche Verkaufszeit beträgt 7,66h !")
```

---

## (Matrizen)

```yaml
type: NormalExercise
key: 3e48f500af
xp: 100
```

Matrizen sind eine rechteckige Anordnung (Tabelle) von Elementen. In R können komplexe Matrixoperationen einfach und effizient durchgeführt werden. In der Statistik werden häufig Matrixberechnungen angewandt (de Vries/Meys 2018).

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

Bislang war immer von einem Vektor die Rede. Des Weiteren gibt es noch Matrizen, die sehr häufig Anwendung finden. Aufgrund der Kürze der Einführung in diesem Kurs kommen wir direkt zu **Data Frames**:

Datensätze bestehen sehr häufig aus unterschiedlichen Datentypen (Produktnamen, Preis, Datum der Herstellung). In eine Matrix bekommen Sie die Daten nur, wenn Sie alles in Text umwandeln, was die Auswertung erschwert. Geeigneter sind da Data Frames, ein Datenobjekt, in dem Sie alle Daten unterschielichen Typs speichern können (de Vries/Meys 2018).

- Struktur und Datentyp anzeigen lassen: str()
- Anzahl der Zeilen bzw. Spalten ausgeben lassen: nrow() bzw. ncol()


`@instructions`
Der Datensatz aus dem Unternehmen Bambergus, der aus der zentralen Kundendatenbank stammt, enthält verschiedene Kundeninformationen.
Der Datensatz wurde schon eingelesen und ist der Variable **Kundendaten** zugewiesen worden.

1. Was beinhaltet der Datensatz an Informationen, bzw. welchen Datentypen kommen vor?
2. Wie viele Kunden sind im Kundendatensatz aufgelistet, wenn Sie davon ausgehen, dass es keine doppelten Kunden gibt?

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

## (Lists)

```yaml
type: NormalExercise
key: 58ec510adf
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

## Einkauf für die Feier

```yaml
type: NormalExercise
key: 547d116662
xp: 100
```

Variablenzuweisung

Ein grundlegendes Konzept in der (statistischen) Programmierung sind Variablen.

Eine Variable ermöglicht es einen Wert (z.B. 4) oder ein Objekt (z.B. Funktionsbeschreibung) in R zu speichern. Später können Sie den Namen der Variable nutzen, um einfach auf den Wert oder das Objekt zuzugreifen, die innerhalb dieser Variablen hinterlegt sind.

So können Sie der Variable my_var den Wert 4 zuweisen: my_var <- 4

`@instructions`
Sie haben eine Feier bevorstehen: 
- x ist die Anzahl der alkoholischen Getränke (alc)
- y ist die Anzahl der nicht-alkolischen Getränke (nonalc)

Weisen Sie bitte den Variablen x und y den passenden Text der Getränkesorte zu:

`@hint`


`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Alkolische Getränke

# Nicht-alkolische Getränke

# Ausgabe Alkohol

```

`@solution`
```{r}
# Alkolische Getränke
x <- "alc"
# Nicht-alkolische Getränke
y <- "nonalc"
# Augabe Menge Alkohol
print("alc")
```

`@sct`
```{r}
ex() %>% check_object("x") %>% check_equal("alc")
ex() %>% check_object("y") %>% check_equal("nonalc")
ex() %>% check_code(c("print(x)", "x", print("alc"), "alc"), fixed = TRUE)
ex() %>% check_output("alc", fixed=TRUE, missing_msg= "Da stimmt etwas nicht!")
success_msg("Ja, genau - es sieht so aus als hätten Sie die Variablenzuweisung verstanden!")
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
success_msg("Gute Arbeit! Yeah richtig gut gemacht!")
```

---

## Erzeugen von Vektoren

```yaml
type: NormalExercise
key: bd8c85316c
xp: 100
```

Vektoren erzeugen und kombinieren:
- Ein Vektor ist die einfachste Datenstruktur in R. Als "einzelnes Objekt, das aus einer Ansammlung von Dingen besteht" wird ein Vektor im R-Handbuch definiert. Es ist die kleinstmögliche Dateneinheit in R (de Vries/Meys 2018). Wir behandeln hier zum Einstieg numerische Vektoren, also Vektoren, die alle Arten von Zahlen enthalten können.

Vektoren erzeugen: 

Um einen Vektor mit einer Folge von Zahlen von 1 bis 3 zu erzeugen und ihn zuzuweisen:  c(1,2,3) oder kürzer c(1:3)
- first_vec <- c(1:3).

`@instructions`
1. Erstellen Sie einen Vektor, der die Zahlen von 1 bis 6 beinhaltet und weisen Sie ihm bitte den Namen open.vec zu. Die Zahlen stehen jeweils für einen Verkaufstag (1= Montag).
2. In dem Vektor sell.time ist die Verkaufszeit für jeden Verkaufstag hinterlegt. Lassen Sie sich bitte den Vektor ausgeben, um zu bestimmen, welcher Verkaufstag der zeitlich längste ist.
3. Am Freitag wurden 5103 Euro Umsatz generiert. Wie viel wurde pro Stunde umgesetzt?
4. Berechnen Sie bitte die tägliche durchschnittliche (mean) Verkaufszeit pro Verkaufstag.

`@hint`
Schauen Sie sich die Beispiele an. Verwenden Sie diese Schreibweise: Variable <- (Zahl:Zahl)

`@pre_exercise_code`
```{r}
sell.time <- c(8,8,8,8,9,6)
```

`@sample_code`
```{r}

```

`@solution`
```{r}
#1. Erstellen Sie einen Vektor, der die Zahlen von 1 bis 6 beinhaltet und weisen Sie ihm bitten den Namen open.vec zu:
open.vec <- c(1,2,3,4,5,6)

#2. Berechnen Sie den Durchschnitt (mean) des Vektors sell.time und weisen Sie ihm bitte mean_time zu:
mean_time <- mean(sell.time)
```

`@sct`
```{r}
ex() %>% check_object("open.vec") %>% check_equal("c(1,2,3,4,5)", "c(1:5)")
ex() %>% check_object("mean_time") %>% check_equal("mean(sell.time)")
ex() %>% check_object("mean_time") %>% check_equal(8)
success_msg("Ja, genau - es sieht so aus als hätten Sie das Erzeugen von Vektoren verstanden! Die durschnittliche Arbeitszeit an den Arbeitstagen beträgt 7h") 

```
