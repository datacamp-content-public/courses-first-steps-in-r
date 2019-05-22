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

Die Hauptfunktionen von DataCamp

Die linke Funktionsseite:
- 1) Hier im **Exercisebereich** wird immer die grundlegende Theorie dargestellt sein, die dann direkt in der Übung angewendet wird. 
- 2) Im Bereich der **Instruktion** bekommen Sie die Erläuterung, was genau Ihre Aufgabe ist, die Sie anschließend lösen sollen. 
- 3) Die **Hints** können Sie nutzen, wenn Sie nicht mehr weiter kommen und einen Hinweis benötigen.

Die rechte Funktionsseite:
- 4) **script.R** ist ihre Kommandozeile mit der Sie Ihre Befehle und Ihren Code in der Programmiersprache R eingeben.
- 5) Mithilfe des Buttons **Run Code** kompilieren Sie nur den Code mit **Submit Answer** führen Sie ihn aus.
- 6) Die **Console** ist in diesem Fall eine Oberfläche in der Sie sehen können, wie Ihr geschriebener Code ausgeführt wird und welche Ausgaben er liefert. 

Lasst uns mit der ersten Aufgabe starten! Let´s go!

`@instructions`
Hallo und herzlich Willkommen,

Sie sind unser/e neue/r MitarbeiterIn in der **Abteilung Business Intelligence & Data Analytics** und befassen sich das erste Mal mit der Programmiersprache R. Ihr Chef Herr Müller hat Ihnen verschiedene Aufgaben gegeben - nun fangen wir aber erstmal leicht an. 

![](https://assets.datacamp.com/production/repositories/4810/datasets/44f5b387423e2b1a9a47c24d837c1bd4f3184ee0/IT_Mitarbeiter.jpg)

- Wir fangen mit dem Programm an mit dem fast alle Programmierbücher starten:
	- Dafür schreiben Sie bitte: **print("Hello World!")** in das Skript und drücken auf 'Submit Answer'.

`@hint`
Keine Angst - einfach print("Hello World!") in das Skript schreiben und auf 'Submit Answer' drücken.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Ihr erstes Programm: "Hello World!"

```

`@solution`
```{r}
# Ihr erstes Programm: "Hello World!"
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

R kann in seiner Basisfunktion als Rechner verwendet werden. Beachten Sie folgende arithmetische Rechenoperatoren:	 

```
 Addition: + 
 Subtraktion: - 
 Multiplikation: *
 Division: / 
 Potenzierung: ^
 Modulo: %%
```
 
Der Operator Modulo (%%) liefert den Rest der Division der linken Zahl durch die rechte Zahl. Z.B.: 7 %% 2 ist 1.

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
Im Editor auf der rechten Seite gibt es einige Beispiel-Codes. Beachten Sie, dass es Unterschiede in den Zeilen gibt - sie beinhalten Code und mit dem **'#'** werden Kommentare gekennzeichnet.

- 1) Sie sollen die Umsätze der letzten drei Monate zusammenrechnen und somit den Umsatz für das Quartal Q1 erstellen. Fügen Sie bitte eine weitere Codezeile, die Rechnung, hinzu und klicken Sie danach auf "Submit Answer".

```
Umsatz in €: Jannuar 234000 | Februar 320000 | März 294000
```

`@hint`
Stellen Sie sicher, dass Sie die Summe aus 234000 + 320000 + 294000 in einer neuen Zeile eingefügt haben. Starten Sie die Zeile nicht mit einem '#'-Zeichen, ansonsten wird der geschriebene Code nicht wie gewünscht ausgeführt, da damit Kommentare gekennzeichnet werden!

`@sample_code`
```{r}
# Beispielcode Addition 
67+78
#1.Quartalsumsatz Q1:

```

`@solution`
```{r}
# Beispielcode Addition 
67+78
# Quartalsumsatz Q1:
234000 + 320000 + 294000
```

`@sct`
```{r}
#ex() %>% check_output(145, fixed=TRUE, missing_msg= "So ist das nicht richtig - Sie müssen sich verrechnet haben!")
ex() %>% check_output(848000, fixed=TRUE, missing_msg="Sie müssen sich verrechnet haben. Beachten Sie auch mögliche Tippfehler!")
success_msg("Ja, genau - der Umsatz im ersten Quartal beträgt 848000€!")
```

***

```yaml
type: NormalExercise
key: dfd9aea716
xp: 20
```

`@instructions`
- 2. Sie hatten im Quartal Q1 einen Umsatz von 848000€ zuerst ausgegeben. Aufgrund eines Forderungsausfalles von 42800€ müssen diese am Umsatz berücksichtigt werden.

`@hint`
Hier müssen Sie nur zwei Werte voneinander substrahieren.

`@sample_code`
```{r}
# Rückstellung berücksichtigen

```

`@solution`
```{r}

848000-42800
```

`@sct`
```{r}
ex() %>% check_output(805200, fixed=TRUE, missing_msg= "So ist das nicht richtig - beachten Sie Tippfehler!")
success_msg("Richtig! Wir haben nun einen Umsatz in Q1 von 805200€")
```

***

```yaml
type: NormalExercise
key: bfa213b421
xp: 20
```

`@instructions`
- 3. Es sind auf den Umsatz von 295005€ im Januar eine Umsatzsteuer in Höhe von 56050.95€ aufgeschlagen worden. Wie viel Prozent an Umsatzsteuer wurden zur späteren Weitergabe an den Verbraucher aufgeschlagen, wenn die gesamte Steuer weitergegeben wurde? Geben Sie bitte das **Ergebnis in Prozent** aus!

`@hint`
Schauen Sie nochmal konkret auf Ihre Berechnung und überlegen Sie sich, wie Sie eine Verhältnisgleichung aufstellen. Es kann Ihnen helfen, an den Dreisatz aus Ihrer Schulzeit zu denken. Beachten Sie, dass in R anstatt dem Komma als Dezimaltrennzeichen der Punkt verwendet wird!

`@sample_code`
```{r}
# Ausrechnen der Umsatzsteuer

```

`@solution`
```{r}
56050.95/(295005/100)
```

`@sct`
```{r}
ex() %>% check_output("19", fixed=TRUE, missing_msg="Nicht ganz richtig - beachten Sie Tippfehler!")
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: 33bebf536a
xp: 20
```

`@instructions`
- 4. Die Umsätze sollen in Q2 um 2.2% im Monat steigen. Welche Prognose geben Sie für die Umsatzzahlen am Ende des Q2 ab? Nehmen Sie den  Ausgangswert von 805200€ am Ende von Q1 an.

`@hint`
Beachten Sie, dass die Prozente jeweils im Monat steigen. Beachten Sie, dass in R anstatt dem Komma als Dezimaltrennzeichen der Punkt verwendet wird!

`@sample_code`
```{r}
# Umsatzprognose Q2

```

`@solution`
```{r}

805200*(1.022^3)
```

`@sct`
```{r}
ex() %>% check_output(859520.9, fixed=TRUE, missing_msg="So ist das nicht ganz richtig - haben Sie den monatlichen Umsatzwachstum berechnet und beachtet, dass es sich um 3 Monate handelt?!")
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: MultipleChoiceExercise
key: 1041a8d575
xp: 20
```

`@question`
- 6. Herr Müller braucht für weitere Abrechnungen die Information, an welchem Tag (Zahl) wir uns innerhalb der aktuellen Kalenderwoche befinden. Wir haben heute den 11.05.2019 und das Jahr hat 365 Tage. Es ist also der 131 Tag. 
- An welchem Tag liegen wir in der angebrochenen Kalenderwoche?

**Hinweis:** Da das Ergebnis direkt in die Abrechnung einfließst, ist es die Vorgabe, das Ergebnis mit einer Rechenoperation ausgeben zu lassen.

`@possible_answers`
- [5]
- 6
- 7
- 18

`@hint`
Versuchen Sie es doch mal mit dem Modulo-Operator (%%). Sie können die Console in R verwenden. Modulo bedeutet auch Division mit Rest.

`@sct`
```{r}
#ex() %>% check_code(5, fixed=TRUE, missing_msg= "So ist das nicht ganz richtig, überlegen Sie noch einmal. Sonst haben Sie die Möglichkeit, den Hinweis zu nehmen!")
#success_msg("Richtig - sehr gut!")
```

---

## Variablen

```yaml
type: NormalExercise
key: 547d116662
xp: 100
```

Variablen zuweisen und vergleichen:

Ein grundlegendes Konzept in der (statistischen) Programmierung sind Variablen. Eine Variable ermöglicht es einen Wert (z.B. 5) oder eine Zeichenkette (z.B. "Funktionsbeschreibung") in R zu speichern. Später können Sie den Namen der Variable nutzen, um einfach auf den Wert oder das Objekt zuzugreifen, die innerhalb dieser Variablen hinterlegt sind (de Vries/ Meys 2018, S.45 & 86).
- Beispiel: So können Sie der Variable my_var den Wert 5 zuweisen: **my_var <- 5**

```
Variablen vergleichen:
x == y 		TRUE, wenn x exakt mit y übereinstimmt
x != y 		TRUE, wenn x von y abweicht
x > y  
x >= y
x & y 		x logisch-und y
x | y  		x logisch-oder y
!x    		nicht x
xor(x, y) 	exklusiv x logisch-oder y

```

`@instructions`
Herr Müller bittet Sie sich mit den Quartalszahlen der letzten und aktuellen Quartale vertraut zu machen.

1. Sie sollen nun die Quartalszahlen 2019 aus Q1: 805200€  und Q2: 859520.9€ den Variablen x und y zuordnen, um besser die Werte vergleichen zu können. 
2. In der Variable z wurden die Quartalszahlen aus Q3 & Q4 bereits hinterlegt und zugewiesen. Ist es richtig, dass das letzte Halbjahr 2018 erfolgreicher war als das Halbjahr 2019 sich zu entwickeln scheint, wie Herr Müller vermutet?
3. Berechnen Sie die Differenz aus den zwei Quartalen Q2 (Prognosewert 2019) und Q1 (2019) und weisen Sie Ihre Rechnung der Variablen **d** zu.

`@hint`
Schauen Sie bitte in die Exercisebox. Hier ist die Zuweisung anhand eines Beispiels verdeutlicht. Lesen Sie bitte genau die Instruktionen. Der Wert für Variable z wurde bereits zugewiesen.

`@pre_exercise_code`
```{r}
z <- 1655000
```

`@sample_code`
```{r}
# 1.Q1:

# Q2

# 2.Vergleich der halbjährlichen Umsätze aus 2018 und 2019: 

# 3.Verweisen Sie die Differenz aus Q2 (Prognosewert) und Q1 (2019) der Variable d zu:

```

`@solution`
```{r}
# Q1
x <- 805200
# Q2
y <- 859520.9
# 2.Vergleich der Umsätze
z > (x+y)
# 3.Verweisen Sie die Differenz aus Q2 und Q1 der Variable d zu:
d <- (y-x)
```

`@sct`
```{r}
ex() %>% check_object("x") %>% check_equal(805200)
ex() %>% check_object("y") %>% check_equal(859520.9)
ex() %>% check_output("FALSE", fixed=TRUE, missing_msg= "Da haben Sie etwas falsch verglichen bei Aufgabe 2 oder die Aussage von Herrn Müller nicht direkt überprüft!")
ex() %>% check_code(c("54320.9", "y-x", "859520.9-805200"), fixed=TRUE, missing_msg= "Da stimmt etwas bei Aufgabe 3. nicht!")
success_msg("Ja, genau - es sieht so aus als hätten Sie die Variablenzuweisung verstanden und Herr Müller lag mit seiner Prognose falsch. Deshalb ist eine Überpüfung anhand von Daten für fundierte Aussagen und unternehmensrelevante Entscheidungen immer notwendig und wird in Zukunft weiter an Bedeutung zunehmen!")
```

---

## Datentypen in R

```yaml
type: TabExercise
key: 0f1fc594d9
xp: 100
```

R arbeitet mit zahlreichen Datentypen und ist sensitiv auf Groß-/Kleinschreibung. Einige der grundlegendsten Datentypen sind:

![Datentypen](https://assets.datacamp.com/production/repositories/4810/datasets/893260b55479a71ff88107db16b1a96fc6bd4116/Basisdatentypen_R.PNG)

**Wichtig:** Zeichenketten werden in "Anführungszeichen" gesetzt.

Von einer kleinen Tochtergesellschaft hat Ihr Chef Herr Müller einen Kundendatensatz zugeschickt bekommen. Er sagt Ihnen, dass die Mitarbeiter dort noch nicht vertraut mit den Datentypen seien. Deswegen müssen Sie sich damit beschäftigen, um dies zu überprüfen.

`@pre_exercise_code`
```{r}
Anzahl_Mitarbeiter <- "Schmidt, Klaus"
```

***

```yaml
type: NormalExercise
key: f3c9691aef
xp: 35
```

`@instructions`
- 1. Die Variable **Anzahl_Mitarbeiter** müsste ein numerischer Basisdatentyp sein. Überprüfen Sie dies bitte.

`@hint`
Schreiben Sie bitte den Code so, damit als Output ein boolescher Wert (TRUE oder FALSE) ausgegeben wird! Schauen Sie in die Tabelle unter **Abfrage (Query)**

`@sample_code`
```{r}
#1.Überprüfung Datentyp Variable Anzahl_Mitarbeiter:

```

`@solution`
```{r}
#1.Überprüfung Variable Anzahl_Mitarbeiter:
is.numeric(Anzahl_Mitarbeiter)
```

`@sct`
```{r}
ex() %>% check_output(c(FALSE, "character"), fixed=TRUE, missing_msg= "Nicht richtig. Schreiben Sie bitte den Code so, damit als Output ein boolescher Wert ausgegeben wird!")
success_msg("Super, es ist keine numerische Variable hinterlegt, da müssen die Mitarbeiter der Tochtergesellschaft etwas falsch zugewiesen haben!")
```

***

```yaml
type: NormalExercise
key: 2a20b35038
xp: 35
```

`@instructions`
- 2. Lassen Sie sich bitte die Variable **Anzahl_Mitarbeiter** ausgeben und wenn nicht die Anzahl von **17** hinterlegt ist, tun Sie dies bitte. Klicken Sie zur Zwischenausgabe auf 'Run Code'.

`@hint`
Eine Zuweisung (<-) funktioniert mit diesem Zeichen in R. Weisen Sie der Variablen den numerischen Wert 17 zu.

`@sample_code`
```{r}
#1.numerische Variable?
is.numeric(Anzahl_Mitarbeiter)
#class(Anzahl_Mitarbeiter) funktioniert auch, gibt direkt den Basisdatentyp aus. Dies können Sie an anderer Stelle verwenden.
#2.Ausgabe + Zuweisung



```

`@solution`
```{r}
#2.1 Ausgabe und ggf. neue Zuweisung
print(Anzahl_Mitarbeiter)

Anzahl_Mitarbeiter <- 17
```

`@sct`
```{r}
ex() %>% check_code(c("Anzahl_Mitarbeiter <- 17", "17->Anzahl_Mitarbeiter"), fixed=TRUE, missing_msg= "Nicht richtig. Schreiben Sie bitte den Code so, damit als Output 17 ausgeben wird!")
success_msg("Super, nun ist der richtige Wert zugewiesen worden!")
```

***

```yaml
type: NormalExercise
key: 08e4ebd18f
xp: 30
```

`@instructions`
- 3. Ihr Chef Herr Müller hat für den Mitarbeiter Maximilian Flix ein neues Büro renovieren lassen. Nennen Sie das Büro **Office_33** bitte in **Nordwand** um.

`@hint`
Verweisen Sie auf die Variable Office_33 einfach den neuen Namen. Beachten Sie, dass Nordwand eine Zeichenkette/String ist.

`@sample_code`
```{r}
#1.numerische Variable?
is.numeric(Anzahl_Mitarbeiter)
#2.Ausgabe + Zuweisung
print(Anzahl_Mitarbeiter)
Anzahl_Mitarbeiter <- 17
#3.Umbenennung Büro

```

`@solution`
```{r}

Office_33 <- "Nordwand"
```

`@sct`
```{r}
ex() %>% check_code(c(Office_33 <- "Nordwand", "Nordwand"-> Office_33), fixed=TRUE, missing_msg= "Da haben Sie etwas nicht richtig zugewisen. Verweisen Sie auf die Variable Office_33 den neuen Namen")
success_msg("Super - weiter geht´s, wir haben keine Zeit zu verlieren!")
```

***

```yaml
type: MultipleChoiceExercise
key: 87f538b93c
```

`@question`
Was ist "53.Stock" für ein Basisdatentyp?
- 1: Es ist ein booleischer Wert - logical.
- 2: Es ist eine Ganzzahl oder Fließkommazahl - numeric.
- 3: Es ist eine Zeichenkette - character.
- 4: Es ist eine Kategorie - factor.

`@possible_answers`
- 1
- 2
- [3]
- 4

`@hint`
Beachten Sie die Anführungszeichen.

`@sct`
```{r}
#ex() %>% check_code(3, fixed=TRUE, missing_msg="Leider nicht richtig, überlegen Sie noch einmal!")
#success_msg("Richtig - es ist eine Zeichenkette (String), da der Wert in Anführungszeichen notiert ist")
```

---

## Vektoren

```yaml
type: TabExercise
key: 2a988ba927
xp: 100
```

Ein Vektor ist die einfachste Datenstruktur in R. Als "einzelnes Objekt, das aus einer Ansammlung von Daten besteht" wird ein Vektor im R-Handbuch definiert. Wir behandeln in dieser Einheit zum Einstieg nur numerische Vektoren, also Vektoren, die alle Arten von Zahlen enthalten können (de Vries/Meys 2018).

Um einen Vektor mit einer Folge von Zahlen von 1 bis 3 zu erzeugen:  
```
c(1,2,3) oder kürzer c(1:3)
```

Wichtige Befehle:

**str()**: Typ eines Vektors bestimmen und Überblick verschaffen.

**mean()**: Durchschnitt ausrechnen.

`@pre_exercise_code`
```{r}
sell.time <- c(8,8,8,8,9,6)
revenue.day <- c(2700, 3500, 4200, 4700, 5103, 3300)
```

***

```yaml
type: NormalExercise
key: ddc67f62d4
xp: 25
```

`@instructions`
Sie sollen als Mitarbeiter der Business Intelligence & Data Analyticsabteilung erneut der kleinen Tochtergesellschaft zuarbeiten und analysieren dazu die Verkaufszeiten, den Umsatz pro Stunde und vergleichen diese auf Profitabilität.

- 1. Erstellen Sie einen Vektor, der die Zahlen von 1 bis 6 beinhaltet und weisen Sie ihm bitte den Variablennamen **open.vec** zu. Die Zahlen stehen jeweils für einen Verkaufstag (1 = "Montag")

`@hint`
Schauen Sie bitte in die Exercisebox dort sind Beispiele gegeben.

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
- 2. In dem Vektor **sell.time** ist die Verkaufszeit für jeden Verkaufstag hinterlegt. Lassen Sie sich bitte die Informationen über Typ und Struktur des Vektors **sell.time** ausgeben. Beurteilen Sie bitte, ob dieser nur numerische Zahlen enthält und welcher Tag der zeitlich längste ist.

`@hint`
Die Funktion **str()** haben Sie in der Kontextbeschreibung gegeben.

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
ex() %>% check_code("str(sell.time)", fixed=TRUE, missing_msg="Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau. Die Funktion str() ist sehr hilfreich und verschafft Ihnen einen guten Überblick über den Vektor. Es ist nützlich, den Befehl immer im Hinterkopf zu behalten!")
```

***

```yaml
type: NormalExercise
key: fb1812faa3
xp: 25
```

`@instructions`
- 3. Am Freitag wurden 5103 Euro Umsatz generiert. Wie viel wurde pro Stunde umgesetzt? Rechnen Sie es bitte aus.

`@hint`
Eine Divisionsaufgabe - denken Sie nicht kompliziert und tippen Sie es ein.

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
ex() %>% check_output(567, fixed=TRUE, missing_msg="Nicht richtig, da haben Sie sich verrechnet!")
success_msg("Richtig. Am Freitag wurden 567€ Umsatz pro Stunde erwirtschaftet!")
```

***

```yaml
type: NormalExercise
key: 05a1752bca
xp: 25
```

`@instructions`
- 4. Berechnen Sie bitte die tägliche durchschnittliche Verkaufszeit pro Verkaufstag in der Woche.

`@hint`
Benutzen Sie die Funktion aus der Exercisebox und verwenden Sie die richtige Variable.

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
ex() %>% check_output(7.833333, fixed=TRUE, missing_msg="Nicht ganz richtig!")
success_msg("Richtig - die durchnittliche tägliche Verkaufszeit beträgt 7,83 h!")
#ex() %>% check_code(c("47/6","mean(sell.time)", "(8+8+8+8+9+6)/6)"), fixed=TRUE, missing_msg="Nicht ganz richtig!")
#success_msg("Richtig - die durschnittliche tägliche Verkaufszeit beträgt 7,83 h!")
```

---

## Matrizen

```yaml
type: TabExercise
key: ebe932dc2c
xp: 100
```

Matrizen sind rechteckige, zweidimensionale Anordnungen von Elementen, wie Tabellen. In R können Matrixoperationen einfach und effizient durchgeführt werden. Anhand von Matrizen können Sie im Gegensatz zu Vektoren nun mehrere Zeilen in ein und derselben Matrix speichern (de Vries/Meys 2018).

Vektoren in eine Matrix zusammenführen: 
- **rbind():** Funktion mit der Vektoren zu Zeilen ein und derselbe Matrix zusammengefügt werden können. *Matrix <- rbind(Vektor, Vektor)
- **cbind():** Funktion mit der Vektoren als Spalten einer Matrix zusammengefügt werden.

Werte einer Matrix ersetzen:
- Um den Wert in der dritten Zeile und zweiten Spalte der Matrix zu 5 zu ändern: my.matrix[3,2] <- 5

Zeilen- und Spaltennamen verändern: 
- Zeilennamen verändern: Bsp. **rownames(Matrix)** <- c("Region", "Umsätze")
- Spaltennamen verändern: Bsp. **colnames(Matrix)** <- c("Januar", "Februar")

`@pre_exercise_code`
```{r}
report.weeksales <- matrix(1:18, ncol=6)
report.final <- matrix(1:18, ncol=6)
sell.time <- c(8,88,8,8,9,6)
revenue.day <- c(2700, 3500, 4200, 4700, 5103, 3300)
average.byday <- c(2700/8, 3500/8, 4200/8, 4700/8, 5103/9, 3300/6)
```

***

```yaml
type: NormalExercise
key: 45beaefb5a
xp: 35
```

`@instructions`
Herr Müller bittet Sie einen Report mit dem Namen **report.weeksales** für die Tochterfirma zu erstellen.

- 1. Ihre Aufgabe ist es eine Matrix (Tabelle) aus den Vektoren **sell.time und revenue.day** zu erstellen und der Variable vom Typ Matrix **report.weeksales** zuzuordnen. Schauen Sie, ob Sie es richtig gemacht haben mit der Ausgabe in der Console.

`@hint`
Schauen Sie bitte in die Exercisebox und verwenden Sie bitte die Funktion um Zeilenvektoren zusammen zu führen und verweisen (<-) Sie diese auf report.weeksales.

`@sample_code`
```{r}
# report.weeksales

```

`@solution`
```{r}

report.weeksales <- rbind(sell.time, revenue.day)
```

`@sct`
```{r}
ex() %>% check_code(c("report.weeksales <- rbind(sell.time, revenue.day)", "rbind(sell.time, revenue.day) -> report.weeksales"), fixed=TRUE, missing_msg="Da stimmt etwas bei dem Erstellen der Matrix nicht. Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau - Schauen Sie sich gern Ihre selbst erstellte Tabelle an!")

#ex() %>% check_object("report.weeksales") %>% check_equal("rbind(sell.time, revenue.day)", fixed=TRUE, missing_msg="So ist das nicht ganz richtig!")
#success_msg("Ja, genau!")
```

***

```yaml
type: NormalExercise
key: 66d829cdea
xp: 35
```

`@instructions`
- Sie haben den Report bei Herrn Müller abgegeben. Er kommt auf Sie zu und entgegnet Ihnen, ob Ihnen aufgefallen sei, dass sich noch ein Zahlenfehler eingeschlichen hat.

- 2. Lassen Sie sich die Matrix report.weeksales ausgeben und korrigieren Sie bitte den Report.

`@hint`
Haben Sie den falschen Wert entdeckt, ein Tag hat nur 24h! - Alles darüber ist falsch. report.weeksales[Zeile, Spalte] <- Wert

`@sample_code`
```{r}
# report.weeksales
report.weeksales <- rbind(sell.time, revenue.day)
#2.Ausgabe + Änderung vornehmen

```

`@solution`
```{r}
# Ausgabe
print(report.weeksales)
# Änderung vornehmen
report.weeksales[1,2] <- 8
```

`@sct`
```{r}
ex() %>% check_code(c("report.weeksales[1,2] <- 8","8 -> report.weeksales[1,2]"), fixed=TRUE, missing_msg="Der Code für die Änderung des Wertes ist nicht korrekt! Haben Sie die richtige Indizierung zur Korrektur des Wertes ausgewählt?") 
success_msg("Ja, genau - sonst wären falsche Umsatzzahlen an die Verkaufsniederlassung weitergegeben worden!")

#Wirft bei Check object die Lösung aus
#ex() %>% check_object("report.weeksales[1,2]") %>% check_equal(8, fixed=TRUE, missing_msg="Der Code für die Änderung des Wertes ist nicht korrekt!")
#success_msg("Ja, genau - da war wohl jemand unaufmerksam. Gut, dass Sie es geändert haben, sonst wären falsche Umsatzzahlen an die Verkaufsniederlassung weitergegeben worden!")
```

***

```yaml
type: NormalExercise
key: fd557c6f5a
xp: 30
```

`@instructions`
- 3. Sie hatten für Freitag schon den durchschnittlichen Umsatz pro Stunde ausgerechnet. In dem Vektor **average.byday** wurde der Umsatz pro Stunde für alle sechs Verkaufstage errechnet. Fügen Sie dem Report bitte die Information des Vektors hinzu, damit der Wochenreport vollständig ist und weisen Sie den neuen Report bitte der Variablen **report.final** zu.

`@hint`
Bitte einen weiteren Vektor average.byday der Matrix hinzufügen. Die Funktion rbind() hatten Sie bereits in Teil 1 dieser Aufgabe verwendet.

`@sample_code`
```{r}
# report.weeksales
report.weeksales <- rbind(sell.time, revenue.day)
# Ausgabe + Änderung vornehmen
print(report.weeksales)
report.weeksales[1,2] <- 8
# Vektor hinzufügen


```

`@solution`
```{r}
report.final <- rbind(sell.time, revenue.day, average.byday) 
```

`@sct`
```{r}
ex() %>% check_code(c("report.final <- rbind(sell.time, revenue.day, average.byday)","report.final <- rbind(report.weeksales, average.byday)"), fixed=TRUE, missing_msg= "Haben Sie den Vektor dem richtigen Teil der Tabelle zugewiesen? Verwenden Sie dazu bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau - der final Report ist fast fertig!")

#ex() %>% check_object("report.final") %>% check_equal(c("rbind(sell.time, revenue.day, average.byday)", "report.final <- rbind(report.weeksales, average.byday)"), fixed=TRUE, missing_msg="Der Code für die Änderung des Wertes ist nicht korrekt!")
#success_msg("Richtig!")
```

***

```yaml
type: NormalExercise
key: 7a6e4f697b
```

`@instructions`
Nun ist der Report für die Tochtergesellschaft schon fast fertig. Es fehlt noch eine eindeutige Benennung, damit dem Management der Tochtergesellschaft auf einen schnellen Blick ersichtlich ist, was dargestellt und analyisiert wurde. 

- 4. Bitte benennen Sie bei dem erstellten finalen Report die Zeilen- und Spaltennamen:
		- **Sales time in h, Revenue, Revenue per hour **
        - **Monday, Tuesday, Wednesday, Thursday, Friday, Saturday**

`@hint`
Schauen Sie dazu in die Exercisebox. Die Beispiele verdeutlichen die notwendige Programmierung sehr gut. Achten Sie darauf, dass die Bennenungen Zeichenketten sind.

`@sample_code`
```{r}
# report.weeksales
report.weeksales <- rbind(sell.time, revenue.day)
# Ausgabe + Änderung vornehmen
print(report.weeksales)
report.weeksales[1,2] <- 8
# Vektor hinzufügen
report.final <- rbind(sell.time, revenue.day, average.byday) 
# Tabelle benennen


```

`@solution`
```{r}
# Zeilennamen benennen
rownames(report.final) <- c("Sales time in h", "Revenue", "Revenue per hour")
## Spaltennamen bennen
#colnames(report.final) <- c("Monday","Tuesday", "Wednesday", "Thursday", "Friday", "Saturday")
```

`@sct`
```{r}
ex() %>% check_code(rownames(report.final) <- c("Sales time in h", "Revenue", "Revenue per hour"), fixed=TRUE, missing_msg="Haben Sie beachtet, dass die Benennungen Zeichenketten sind und dementsprechend gekennzeichnet werden müssen?") 
success_msg("Ja, genau! So behalten Sie die Übersicht und auch andere können Ihre Ergebnisse leichter nachvollziehen!")
ex() %>% check_code(colnames(report.final) <- c("Monday","Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"), fixed=TRUE, missing_msg=" Haben Sie alle Wochentage ohne Tippfehler und als Zeichenkette gekennzeichnet erstellt? Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung") 
success_msg("Ja, genau - so behalten Sie die Übersicht und auch andere können Ihre Ergebnisse leichter nachvollziehen!")
```

---

## Listen

```yaml
type: VideoExercise
key: 871247578a
xp: 50
```

`@projector_key`
50052f5ae7dbd75eaf808625828fa0a0

---

## Data Frames

```yaml
type: TabExercise
key: 0675d8c8f5
xp: 100
```

Nach den Listen kommen wir zur Spezialform von Listen, zu **Data Frames**. 
Data Frames sind Listen mit Vektoren gleicher Länge, die bei der Datenanalyse in R sehr häufig Anwendung finden, da in einem Data Frame unterschiedliche Datentypen gespeichert werden können  (Grolemund 2019, S.55).

Nützliche Funkionen: 
- **nrow() bzw. ncol()**: Anzahl der Zeilen bzw. Spalten
- **names()**: Funktionen zum Abrufen oder Einstellen der Namen eines Objekts
- **colnames()**: Abrufen oder setzen der Zeilen- oder Spaltennamen eines matrixartigen Objektes
- **head()** | **tail()**: Liefert den ersten oder letzten Teil eines Datenobjektes
- **str()**: Erstellt eine kompakte Darstellung der internen Struktur
- **summary()**: Generische Funktion für Ergebniszusammenfassungen

`@pre_exercise_code`
```{r}
Kundendaten <- read.csv2("https://assets.datacamp.com/production/repositories/4810/datasets/31e25bf7206a508aa8681c19698e57afc52ab492/dataMay-3-2019.csv")
```

***

```yaml
type: MultipleChoiceExercise
key: a05461fbaa
xp: 50
```

`@question`
Warum ist es nicht möglich diese Tabelle mit weiteren 3500 Zeilen in eine Matrix zu speichern?

![Beispiel](https://assets.datacamp.com/production/repositories/4810/datasets/81e60fc1e3769bcf2010d82dec9b050ab3c87ca3/Data_frame_bsp..PNG.png)

1. weil der Datensatz unterschiedliche Datentypen nämlich Zeichenketten (character) und numerische Werte (numeric) enthält.
2. weil der Datensatz unterschiedliche Datentypen nämlich numerische Werte und boolesche Werte enthält.
3. weil der Datensatz zu groß ist und deswegen nicht geladen werden kann.
4. er lässt sich ohne weitere Bearbeitung in eine Matrix speichern.

`@possible_answers`
- [1]
- 2
- 3
- 4

`@hint`


`@sct`
```{r}
ex() %>% check_code(1, fixed=TRUE, missing_msg="Leider nicht richtig, es kommen in dem Datensatz keine boolschen Werte vor!")
success_msg("Richtig - in Matrizen können nur gleiche Datentypen gespeichert werden. In Data Frames können Elemente unterschiedlichen Typs gleicher Zeilenlänge gespeichert werden. Innerhalb der Spalten müssen aber die Datentypen gleich sein")

#ex() %>% check_code(2, fixed=TRUE, missing_msg="Leider nicht richtig, es kommen in dem Datensatz keine boolschen Werte vor!")
#success_msg("")
#ex() %>% check_code(3, fixed=TRUE, missing_msg="Leider nicht richtig, dies ist für R kein Problem!")
#success_msg("")
#ex() %>% check_code(4, fixed=TRUE, missing_msg="Leider nicht richtig, unterschiedliche Datentypen lassen sich nicht einer Matrix speichern. #Überlegen Sie noch einmal!")
#success_msg("")
```

***

```yaml
type: NormalExercise
key: 968db7b3b5
xp: 50
```

`@instructions`
Der Datensatz aus dem Unternehmen Bambergus, der aus der zentralen Kundendatenbank stammt, enthält verschiedene Kundeninformationen.
Er wurde eingelesen und der Variable **Kundendaten** zugewiesen.

1. Wie viele Kunden sind im Kundendatensatz aufgelistet, wenn Sie annehmen, dass es keine doppelten Kunden in der Tabelle gibt?

`@hint`


`@sample_code`
```{r}
# Anzahl Kunden

```

`@solution`
```{r}

nrow(Kundendaten)
```

`@sct`
```{r}
ex() %>% check_output(100, fixed=TRUE, missing_msg="So ist das nicht richtig - vielleicht haben Sie auch nur eine Ausgabefunktion vergessen. Ihr Ziel ist es, dass die Anzahl der Kunden als Ausgabe in der Konsole erscheinen")
success_msg("Hervorragend - so einfach bekommt man an ein Ergebnis!")
```

***

```yaml
type: NormalExercise
key: 71a30c036d
```

`@instructions`


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

## Visualisierung

```yaml
type: NormalExercise
key: e826bcc1cb
xp: 100
```



`@instructions`


`@hint`


`@pre_exercise_code`
```{r}
sell.time <- c(8,8,8,8,9,6)
revenue.day <- c(2700, 3500, 4200, 4700, 5103, 3300)
average.byday <- c(2700/8, 3500/8, 4200/8, 4700/8, 5103/9, 3300/6)
report.wochenverkaeufe <- rbind(sell.time, revenue.day, average.byday)
rownames(report.wochenverkaeufe) <- c("Verkaufszeit in h", "Umsatz", "Umsatz pro Stunde")
colnames(report.wochenverkaeufe) <- c("Montag", "Dienstag", "Mittwoch", "Donnerstag", "Freitag", "Samstag")
report.final <- report.wochenverkaeufe
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

## Wrap up. Haben Sie es verstanden?

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
