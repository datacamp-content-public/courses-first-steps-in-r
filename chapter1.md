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
- 1) Hier im **Exercisebereich** wird immer die grundlegende Theorie dargestellt sein, die dann direkt in der Übung angewendet wird. - 
- 2) Im Bereich der **Instruktion** bekommen Sie die Erläuterung, was genau Ihre Aufgabe ist, die Sie anschließend lösen sollen. 
- 3) Die **Hints** können Sie nutzen, wenn Sie nicht mehr weiter kommen und einen Hinweis benötigen.

Die rechte Funktionsseite:
- 4) **script.R** ist ihre Kommandozeile mit der Sie Ihre Befehle und Ihren Code in der Programmiersprache R eingeben.
- 5) Mithilfe des Buttons **RunCode** kompilieren Sie nur den Code mit **Submit Answer** führen Sie ihn aus.
- 6) Die **Console** ist in diesem Fall eine Oberfläche in der Sie sehen können, wie Ihr geschriebener Code ausgeführt wird und welche Ausgaben er liefert. 

Lasst uns mit der ersten Aufgabe starten! Let´s go!

`@instructions`
Hallo und herzlich Willkommen,

Sie sind unser/e neue/r MitarbeiterIn in der IT-Abteilung und befassen sich das erste Mal mit der Programmiersprache R. Ihr Chef Herr Müller hat Ihnen verschiedene Aufgaben gegeben - nun fangen wir aber erstmal leicht an. 

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
 - Addition: + 
 - Subtraktion: - 
 - Multiplikation: * 
 - Division: / 
 - Potenzierung: ^
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
Im Editor auf der rechten Seite gibt es bereits einige Beispiel-Codes. Beachten Sie, dass es Unterschiede in den Zeilen gibt - sie beinhalten Code und mit dem **'#'** werden Kommentare gekennzeichnet.

- 1) Sie sollen die Umsätze der letzten drei Monate zusammenrechnen und somit den Umsatz für das Quartal Q1 erstellen. Fügen Sie bitte eine weitere Codezeile hinzu, fügen Sie Ihre Rechnung ein und klicken Sie danach auf "Submit Answer". Schauen Sie anschließend bitte in die Console.

```
Umsatz: Jannuar 234000 | Februar 320000 | März 294000
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
- 2. Sie hatten im Quartal Q1 einen Umsatz von 848.000€ zuerst ausgegeben. Aufgrund eines Forderungsausfalles von 42800€ müssen diese am Umsatz berücksichtigt werden.

`@hint`
Hier müssen Sie nur zwei Werte voneinander subtrahieren.

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
ex() %>% check_output(805200, fixed=TRUE, missing_msg="So ist das nicht richtig - beachten Sie Tippfehler!")
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: bfa213b421
xp: 20
```

`@instructions`
- 4. Es sind auf den Umsatz von 295005€ im Januar eine Umsatzsteuer in Höhe von 56050.95€ aufgeschlagen worden. Wie viel Prozent an Umsatzsteuer wurden zur späteren Weitergabe an den Verbraucher aufgeschlagen? Runden Sie bitte mit der Funktion round() auf.

`@hint`
Schauen Sie nochmal konkret auf Ihre Berechnung und überlegen Sie sich, wie Sie ein Verhältnisgleichung aufstellen. Denken Sie an den Dreisatz aus Ihrer Schulzeit.

`@sample_code`
```{r}
# Ausrechnen der Umsatzsteuer

```

`@solution`
```{r}
round(56050.95/(295995/100))	
```

`@sct`
```{r}
ex() %>% check_output(c("0.19", "19", "56050.95/(295005/100)"), fixed=TRUE, missing_msg="Nicht ganz richtig - beachten Sie Tippfehler!")
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: 33bebf536a
xp: 20
```

`@instructions`
- 4. Die Umsätze sollen in Q2 um 2.2% im Monat steigen. Welche Prognose geben Sie für die Umsatzzahlen am Ende des Q2 ab? Nehmen Sie den  Ausgangswert von 805200 am Ende von Q1 an.

`@hint`
Beachten Sie, dass in R anstatt dem Komma als Dezimaltrennzeichen der Punkt verwendet wird!

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
ex() %>% check_output(859520.9, fixed=TRUE, missing_msg="So ist das nicht ganz richtig - beachten Sie Tippfehler!")
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: 94b44944a6
xp: 20
```

`@instructions`
- 5. Herr Müller braucht für weitere Abrechnungen die Information, an welchem Tag (Zahl) wir uns innerhalb der aktuellen Kalenderwoche befinden. Wir haben heute den 11.05.2019 und das Jahr hat 365 Tage. Es ist also der 131 Tag. An welchem Tag liegen wir in der angebrochenen Kalenderwoche?

**Hinweis:** Da das Ergebnis direkt in die Abrechnung einfließst, ist es die Vorgabe, das Ergebnis mit einer Rechenoperation ausgeben zu lassen.

`@hint`
Versuchen Sie es doch mal mit dem Modulo-Operator (%%)

`@sample_code`
```{r}
# Tag in der aktuellen Kalenderwoche

```

`@solution`
```{r}
131%%7
```

`@sct`
```{r}
ex() %>% check_output(5, fixed=TRUE, missing_msg="So ist das nicht ganz richtig, achten Sie auf den Hinweis!")
success_msg("Richtig")
```

***

```yaml
type: NormalExercise
key: 713bfa0770
```

`@instructions`
- 6. Herr Müller zeigt strebt ein Umsatzziel für Q3 (2019) von 910000 an. Wie hoch muss dafür das Umsatzwachstum ausfallen, wenn Ende Q2(2019) 859521€ Umsatz vorliegen.

R hält eine riesige Menge von mathematischen Funktionen bereit. 
```
log(x,base = y) Logarithmus von x zur Basis y
exp(x) Exponentailfunktion von x
sqrt(x) Qudratwurzel von x
```

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

***

```yaml
type: MultipleChoiceExercise
key: 6df8493e71
```

`@question`
- 7. Wie lautet das Ergebnis von 11 Modulo 4

`@possible_answers`
- 1
- 2
- [3]
- 9

`@hint`
Das geht im Kopf - hier geht es nun um das Verständnis. Sie können aber auch die Console in R verwenden.

`@sct`
```{r}
ex() %>% check_code(3, fixed=TRUE, missing_msg="Leider nicht richtig, überlegen Sie noch einmal!")
success_msg("Richtig - Sie werden in Zukunft noch öfters den Modulooperator brauchen")
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

Beispiel: So können Sie der Variable my_var den Wert 5 zuweisen: **my_var <- 5**

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

1. Sie sollen nun die Quartalszahlen 2019 aus Q1: 805200  und Q2: 859520.9 den Variablen x und y zuordnen, um besser die Werte vergleichen zu können. 
2. In der Variable z wurden die Quartalszahlen aus Q3 & Q4 hinterlegt. Ist es richtig, dass das letzte Halbjahr 2018 erfolgreicher war als das Halbjahr 2019 sich zu entwickeln scheint, wie Herr Müller vermutet?
3. Berechnen Sie die Differenz aus den zwei Quartalen Q2 (Progosewert 2019) und Q1 2019 und weisen Sie Ihre Rechnung der Variablen **d** zu.

`@hint`


`@pre_exercise_code`
```{r}
z <- 1655000
```

`@sample_code`
```{r}
# 1.Q1

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

## Basisdatentypen in R

```yaml
type: TabExercise
key: 0f1fc594d9
xp: 100
```

R arbeitet mit zahlreichen Datentypen und ist sensitiv auf Groß-/Kleinschreibung. Einige der grundlegendsten Datentypen sind:

![Basisdatentypen](https://assets.datacamp.com/production/repositories/4810/datasets/893260b55479a71ff88107db16b1a96fc6bd4116/Basisdatentypen_R.PNG)

**Wichtig:** Zeichenketten werden in "Anführungszeichen" gesetzt.

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
Von einer kleineren Tochtergesellschaft, die neu eröffnet hat, hat Ihr Chef Herr Müller einen Kundendatensatz zugeschickt bekommen. Herr Müller sagt, dass die Mitarbeiter dort noch nicht vertraut mit den Datentypen seien und Sie sich deswegen genau mit den Basisdatentypen beschäftigen müssen, damit die Mitarbeiter von Ihnen eine Vorlage bekommen können. 
Kontrollieren Sie bitte einzelne Werte hinsichtlich ihrer Basisdatentypen.

- 1. Die Variable **Anzahl_Mitarbeiter** müsste ein numerischer Basisdatentyp sein. Überpüfen Sie dies bitte.

`@hint`
Schreiben Sie bitte den Code so, damit als Output ein boolescher Wert (TRUE oder FALSE) ausgegeben wird! Schauen Sie in die Tabelle unter **Abfrage (Query)**

`@sample_code`
```{r}
#1.Überprüfung des numerischen Datentyps

```

`@solution`
```{r}
#1.Überprüfung des numerischen Datentyps
is.numeric(Anzahl_Mitarbeiter)
```

`@sct`
```{r}
ex() %>% check_output(FALSE, fixed=TRUE, missing_msg= "Nicht richtig. Schreiben Sie bitte den Code so, damit als Output ein boolescher Wert ausgegeben wird!")
success_msg("Super, es ist keine numerische Variable hinterlegt, da müssen die Mitarbeiter der Tochtergesellschaft etwas falsch zugewiesen haben!")
```

***

```yaml
type: NormalExercise
key: 2a20b35038
xp: 35
```

`@instructions`
- 2. Lassen Sie sich bitte die Variable **Anzahl_Mitarbeiter** ausgeben und wenn nicht die Anzahl von **17** hinterlegt ist, tun sie dies bitte. Klicken Sie zur Zwischenausgabe 'Run Code'

`@hint`
Eine Zuweisung (<-) funktiniert mit diesem Zeichen in R. Weisen Sie der Variablen den numerischen Wert 17 zu.

`@sample_code`
```{r}
#1.numerische Variable?
is.numeric(Anzahl_Mitarbeiter)
class(Anzahl_Mitarbeiter) #funktioniert auch, gibt direkt den Basisdatentyp aus.
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
ex() %>% check_code("Anzahl_Mitarbeiter <- 17", fixed=TRUE, missing_msg= "Nicht richtig. Schreiben Sie bitte den Code so, damit als Output 17 ausgeben wird!")
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
Verweisen Sie auf die Variable Office_33 einfach den neuen Namen. Beachten Sie, dass Nordwand ein String ist und folglich in Anführungszeichen gesetz werden muss.

`@sample_code`
```{r}
#1.numerische Variable?
is.numeric(Anzahl_Mitarbeiter)
#2.Ausgabe + Zuweisung
print(Anzahl_Mitarbeiter)
Anzahl_Mitarbeiter <- 17
#3 Umbenennung Büro

```

`@solution`
```{r}

Office_33 <- "Nordwand"
```

`@sct`
```{r}
ex() %>% check_code(Office_33 <- "Nordwand", fixed=TRUE, missing_msg= "Verweisen Sie auf die Variable Office_33 einfach den neuen Namen")
success_msg("Super!")
```

***

```yaml
type: MultipleChoiceExercise
key: 87f538b93c
```

`@question`


`@possible_answers`


`@hint`


`@sct`
```{r}

```

---

## Vektoren

```yaml
type: TabExercise
key: 2a988ba927
xp: 100
```

Ein Vektor ist die einfachste Datenstruktur in R. Als "einzelnes Objekt, das aus einer Ansammlung von Dingen besteht" wird ein Vektor im R-Handbuch definiert. Es ist die kleinstmögliche Dateneinheit in R. Wir behandeln in dieser Einheit zum Einstieg nur numerische Vektoren, also Vektoren, die alle Arten von Zahlen enthalten können (de Vries/Meys 2018).

Um einen Vektor mit einer Folge von Zahlen von 1 bis 3 zu erzeugen:  
```
c(1,2,3) oder kürzer c(1:3)
```

Typ eines Vektors bestimmen und Überblick verschaffen: **str()**

Durchschnitt ausrechnen: **mean()**

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
Sie sollen als neuer Mitarbeiter wieder der kleinen Tochtergesellschaft zuarbeiten und analysieren dazu die Verkaufszeiten, den Umsatz pro Stunde und vergleichen diesen.

- 1. Erstellen Sie einen Vektor, der die Zahlen von 1 bis 6 beinhaltet und weisen Sie ihm bitte den Namen open.vec zu. Die Zahlen stehen jeweils für einen Verkaufstag (1= Montag)

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
- 2. In dem Vektor sell.time ist die Verkaufszeit für jeden Verkaufstag hinterlegt. Lassen Sie sich bitte die Informationen über Typ und Struktur des Vektors sell.time ausgeben. Beurteilen Sie bitte, ob dieser nur numerische Zahlen enthält und welcher Tag der zeitlich Längste ist.

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
ex() %>% check_code("str(sell.time)", fixed=TRUE, missing_msg="Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau!")
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
- 4. Berechnen Sie bitte die tägliche durchschnittliche Verkaufszeit pro Verkaufstag in der Woche.

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
ex() %>% check_output(47/6, fixed=TRUE, missing_msg="Nicht ganz richtig!")
success_msg("Richtig - die durschnittliche tägliche Verkaufszeit beträgt 7,83 h !")
#ex() %>% check_code(c("47/6", "mean(sell.time)"), fixed=TRUE, missing_msg="Nicht ganz richtig!")
#success_msg("Richtig - die durschnittliche tägliche Verkaufszeit beträgt 7,83 h !")
```

---

## Matrizen

```yaml
type: TabExercise
key: ebe932dc2c
xp: 100
```

Matrizen sind rechteckige, zweidimensionale Anordnungen (Tabellen) von Elementen. In R können komplexe Matrixoperationen einfach und effizient durchgeführt werden. In der Statistik werden häufig Matrixberechnungen angewandt (de Vries/Meys 2018).

Vektoren in eine Matrix zusammenführen: 
- **rbind():** Funktion mit der Vektoren zu Zeilen ein und derselbe Matrix zusammengefügt werden können.
- *Matrix <- rbind(Vektor, Vektor)
- **cbind():** Funktion mit der Vektoren als Spalten einer Matrix zusammengefügt werden.

Werte einer Matrix ersetzen:
- Um den Wert in der dritten Zeile und zweiten Spalte der Matrix matrix.eins zu 5 zu ändern: matrix.eins[3,2] <- 5

Um die Übersicht zu behalten und damit auch andere die Ergebnisse nachvollziehen können. Zeilen- und Spaltennamen sinnvoll verändern: 
- Zeilennamen verändern: Beispiel **rownames(Matrix)** <- c("Region", "Umsätze")
- Spaltennamen verändern: Beispiel **colnames(Matrix)** <- c("Januar", "Februar")

`@pre_exercise_code`
```{r}
report.wochenverkaeufe <- matrix(1:18, ncol=6)
report.final <- matrix(1:18, ncol=6)
#sell.day <- c("Montag", "Dienstag", "Mittwoch", "Donnerstag", "Freitag", "Samstag")
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
Anhand von Matrizen können Sie im Gegensatz zu Vektoren nun mehrere Zeilen in ein und derselben Tabelle (Matrix) speichern. 

Herr Müller bittet Sie einen **report.wochenverkaeufe** für die Tochterfirma zu erstellen.

- 1. Ihre Aufgabe ist es eine Tabelle (Matrix) aus den Vektoren **sell.time und revenue.day** zu erstellen und der Variablen **report.wochenverkaeufe** zuzuordnen. Testen Sie, ob Sie es richtig gemacht haben mit der Ausgabe in der Console.

`@hint`


`@sample_code`
```{r}
# report.wochenverkaeufe

```

`@solution`
```{r}

report.wochenverkaeufe <- rbind(sell.time, revenue.day)
```

`@sct`
```{r}
ex() %>% check_code("report.wochenverkaeufe <- rbind(sell.time, revenue.day)", fixed=TRUE, missing_msg="Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau - Schauen Sie sich gern Ihre selbst erstellte Tabelle an!")
```

***

```yaml
type: NormalExercise
key: 66d829cdea
xp: 35
```

`@instructions`
- 2.Sie haben den Report bei Herrn Müller abgeben. Er kommt auf Sie zu und entgegnet Ihnen, ob Ihnen aufgefallen sei, dass sich noch ein Zahlenfehler eingeschlichen hat. Kontrollieren Sie dies und ändern Ihn bitte ab.

- 2.1 Lassen Sie sich die Matrix report.wochenverkaeufe ausgeben.

- 2.2 Ändern Sie einen Fehler ab.

`@hint`


`@sample_code`
```{r}
# report.wochenverkaeufe
report.wochenverkaeufe <- rbind(sell.time, revenue.day)
# Ausgabe

# Änderung vornehmen

```

`@solution`
```{r}
# Ausgabe
print(report.wochenverkaeufe)
# Änderung vornehmen
report.wochenverkaeufe[1,2] <- 8
```

`@sct`
```{r}
ex() %>% check_code("report.wochenverkaeufe[1,2] <- 8", fixed=TRUE, missing_msg="Der Code für die Änderung des Wertes ist nicht korrekt!") 
success_msg("Ja, genau - sonst wären falsche Umsatzzahlen an die Verkaufsniederlassung weitergegeben worden!")
```

***

```yaml
type: NormalExercise
key: fd557c6f5a
xp: 30
```

`@instructions`
- 3. Sie hatten für Freitag schon den durchschnittlichen Umsatz pro Stunde ausgerechnet. In dem Vektor **average.byday** wurde der Umsatz pro Stunde für alle sechs Verkaufstage errechnet. Fügen Sie diesen Vektor bitte noch dem Report hinzu, damit der Wochenreport vollständig ist und weisen Sie die Tabelle bitte der Variablen **report.final** zu.

`@hint`


`@sample_code`
```{r}
# report.wochenverkaeufe
report.wochenverkaeufe <- rbind(sell.time, revenue.day)
# Ausgabe
print(report.wochenverkaeufe)
# Änderung vornehmen
report.wochenverkaeufe[1,2] <- 8
# Umsatz pro Tag hinzufügen

```

`@solution`
```{r}
report.final <- rbind(sell.time, revenue.day, average.byday) 
```

`@sct`
```{r}
ex() %>% check_code(c("report.final <- rbind(sell.time, revenue.day, average.byday)","report.final <- rbind(report.wochenverkaeufe, average.byday)"), fixed=TRUE, missing_msg="Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau!")
```

***

```yaml
type: NormalExercise
key: 7a6e4f697b
```

`@instructions`
Nun ist der Report für die Tochtergesellschaft schon fast fertig. Es fehlt noch eine eindeutige Benennung, damit von der Leitung auf einen schnellen Blick ersichtlich ist, was dargestellt wurde. 

- 4. Bitte nennen Sie bei dem erstellten finalen Report die Zeilennamen in **Verkaufszeit h, Tagesumsatz, Umsatz pro Stunde** und die Spaltennamen in **Montag, Dienstag, Mittwoch, Donnerstag, Freitag, Samstag** um.

`@hint`


`@sample_code`
```{r}
# report.wochenverkaeufe
report.wochenverkaeufe <- rbind(sell.time, revenue.day)
# Ausgabe
print(report.wochenverkaeufe)
# Änderung vornehmen
report.wochenverkaeufe[1,2] <- 8
# Umsatz pro Tag hinzufügen
report.final <- rbind(sell.time, revenue.day, average.byday) 
# Zeilennamen benennen

# Spaltennamen benennen

```

`@solution`
```{r}
# Zeilennamen benennen
rownames(report.final) <- c("Verkaufszeit h", "Umsatz", "Umsatz pro Stunde")
# Spaltennamen bennen
colnames(report.final) <- c("Montag", "Dienstag", "Mittwoch", "Donnerstag", "Freitag", "Samstag")
```

`@sct`
```{r}
ex() %>% check_code(rownames(report.final) <- c("Verkaufszeit h", "Umsatz", "Umsatz pro Stunde"), fixed=TRUE, missing_msg="Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau!")
ex() %>% check_code(colnames(report.final) <- c("Montag", "Dienstag", "Mittwoch", "Donnerstag", "Freitag", "Samstag"), fixed=TRUE, missing_msg="Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau!")
```

---

## Data Frames

```yaml
type: TabExercise
key: 0675d8c8f5
xp: 100
```

Bislang war immer bei zweidimensionalen Tabellen von Matrizen die Rede. Nun kommen wir zu den **Data Frames**:

Datensätze bestehen sehr häufig aus unterschiedlichen Datentypen (Produktnamen, Preis, Datum der Herstellung). In eine Matrix bekommen Sie die Daten nur, wenn Sie alles in Text umwandeln, was die Auswertung erschwert. Geeigneter sind da Data Frames, ein Datenobjekt, in dem Sie alle Daten unterschielichen Typs speichern können (de Vries/Meys 2018).

- **nrow() bzw. ncol()**: Anzahl der Zeilen bzw. Spalten ausgeben lassen: 
- **names()**: Funktionen zum Abrufen oder Einstellen der Namen eines Objekts.
- **colnames()**: Abrufen oder setzen der Zeilen- oder Spaltennamen eines matrixartigen Objekts.
- **head()** | **tail()**: Liefert den ersten oder letzten Teil eines Vektors, einer Matrix, einer Tabelle, eines Datenrahmens oder einer Funktion.
- **str()**: Erstellt eine kompakte Darstellung der internen Struktur eines R-Objekts.
- **summary()**: Ist eine generische Funktion, um Ergebniszusammenfassungen zu erstellen.

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
Warum ist es nicht möglich diese Tabelle in eine Matrix zu speichern?

`@possible_answers`


`@hint`


`@sct`
```{r}

```

***

```yaml
type: NormalExercise
key: 968db7b3b5
xp: 50
```

`@instructions`
Der Datensatz aus dem Unternehmen Bambergus, der aus der zentralen Kundendatenbank stammt, enthält verschiedene Kundeninformationen.
Der Datensatz wurde schon eingelesen und ist der Variable **Kundendaten** zugewiesen worden.

1. Was beinhaltet der Datensatz an Informationen, bzw. welchen Datentypen kommen vor?
2. Wie viele Kunden sind im Kundendatensatz aufgelistet, wenn Sie davon ausgehen, dass es keine doppelten Kunden gibt?

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

***

```yaml
type: NormalExercise
key: 0f3bbf5d27
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

---

## Variablenzuweisung

```yaml
type: NormalExercise
key: b16f728974
xp: 100
```

Variablenzuweisung

Ein grundlegendes Konzept in der (statistischen) Programmierung sind Variablen.

Eine Variable ermöglicht es einen Wert (z.B. 5) oder ein Objekt (z.B. Funktionsbeschreibung) in R zu speichern. Später können Sie den Namen der Variable nutzen, um einfach auf den Wert oder das Objekt zuzugreifen, die innerhalb dieser Variablen hinterlegt sind.

So können Sie der Variable my_var den Wert 5 zuweisen: **my_var <- 5**

`@instructions`
Ihre Aufgabe: 
Vervollständigen Sie bitte den Code im Editor, sodass der Variable x der Wert 105 zugeordnet wird. Schicken Sie dann die Antwort ab. 
Wenn Sie R nach x fragen, wird der vorher zu gewiesene Wert angezeigt.

`@hint`
Der Variable my_var wurde im Beispiel der Wert 5 zugeteilt. Orientieren Sie sich einfach an dieser Vorgehensweise.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Weisen Sie x den Wert 105 zu

# Geben Sie den Wert der Variable x aus

```

`@solution`
```{r}
# Weisen Sie x den Wert 105 zu
x <- 105
# Geben Sie den Wert der Variable x aus
x
```

`@sct`
```{r}
ex() %>% check_object("x") %>% check_equal(105)
ex() %>% check_code(c("print(x)", "x"))
ex() %>% check_output("105", fixed=TRUE, missing_msg="So ist das nicht ganz richtig!")
success_msg("Ja, genau: x <- 105 erzeugt keine Ausgabe, weil R davon ausgeht, dass Sie diese Variable in der Zukunft benötigen! Gehen Sie bitte zur nächsten Aufgabe")
```

---

## Basisdatentypen in R

```yaml
type: NormalExercise
key: bd7572143c
xp: 100
```

R arbeitet mit zahlreichen Datentypen und ist sensitiv auf Groß-/Kleinschreibung. Einige der grundlegendsten Datentypen sind:

- Boolesche Werte oder auch als Wahrheitswerte bezeichnet (TRUE oder FALSE) werden auch 'Logical' genannt.
- Dezimalwerte (z.B. 3.4) werden 'numeric' genannt (z.B. )
- Zeichenketten und Buchstaben (Strings) ("Hallo") werden auch als 'character' bezeichnet.
- Kategorien (A,B,C) werden auch als 'factor' bezeichnet.

**Wichtig:** Zeichenketten werden in "Anführungszeichen" gesetzt.

`@instructions`
Von einer kleineren Tochtergesellschaft, die neu eröffnet hat, hat Herr Müller einen Kundendatensatz zugeschickt bekommen. Ihr Chef Herr Müller sagt, dass die Mitarbeiter dort noch nicht vertraut mit den Datentypen seien und Sie sich deswegen genau mit den Basisdatentypen beschäftigen müssen, damit die Mitarbeiter von Ihnen eine Vorlage bekommen können. 

1. Geben Sie den Wert von Anzahl_Mitarbeiter aus.
 
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
Anzahl_Mitarbeiter <- "Schmidt, Klaus"
Termin <- 2019-09-21
```

`@sample_code`
```{r}
# Ausgabe Anzahl_Mitarbeiter:

# Weisen Sie der Variablen Anzahl_Mitarbeiter den Wert 17 zu:

# Bennen Sie my_office mit der Zeichenkette Nordwand:

# Überprüfen Sie, ob Begrueßungstermin eine Datumsangabe ist:

```

`@solution`
```{r}
# Die Anzahl der Mitarbeiter müsste eine numerische Zahl. Überprüfen Sie dies bitte: 
is.numeric(Anzahl_Mitarbeiter)
# Ausgabe Anzahl_Mitarbeiter:
#print(Anzahl_Mitarbeiter)
# Weisen Sie der Variablen Anzahl_Mitarbeiter den Wert 17 zu:
#Anzahl_Mitarbeiter <- 17
# Weisen Sie my_office die Zeichenkette Nordwand zu:
#my_office <- "Nordwand"
# Überprüfen Sie, ob Begrueßungstermin eine Datumsangabe ist:
#is.Date(Begrueßungstermin)
```

`@sct`
```{r}
#ex() %>% check_code(c("print(my_nummerus)", "my_nummerus"), fixed = TRUE)
#ex() %>% check_output("3", fixed=TRUE, missing_msg="Da stimmt etwas nicht!")
#ex() %>% check_object("my_numeric")   %>% check_equal(54)
#ex() %>% check_object("my_character") %>% check_equal("universe")
#ex() %>% check_object("my_logical")   %>% check_equal("FALSE")
#success_msg("Ja, genau - es sieht so aus als hätten Sie die Basisdatentypen verstanden!")
```

---

## Matrizen

```yaml
type: NormalExercise
key: 3e48f500af
xp: 100
```

Matrizen sind rechteckige, zweidimensionale Anordnungen (Tabelle) von Elementen. In R können komplexe Matrixoperationen einfach und effizient durchgeführt werden. In der Statistik werden häufig Matrixberechnungen angewandt (de Vries/Meys 2018).
Anhand von Matrizen können Sie im Gegensatz zu Vektoren nun mehrere Zeilen in ein und derselben Tabelle (Matrix) speichern.

Vektoren in eine Matrix zusammenführen: 
- **rbind():** Funktion mit der Vektoren zu Zeilen ein und derselbe Matrix zusammengefügt werden können.
- *Matrix <- rbind(Vektor, Vektor)
- **cbind():** Funktion mit der Vektoren als Spalten einer Matrix zusammengefügt werden.

Um die Übersicht zu behalten und damit auch andere die Ergebnisse nachvollziehen können. Zeilen- und Spaltennamen sinnvoll verändern: 
- Zeilennamen verändern: Beispiel **rownames(Matrix)** <- c("Region", "Umsätze")
- Spaltennamen verändern: Beispiel **colnames(Matrix)** <- c("Januar", "Februar")

Werte einer Matrix ersetzen:
- Um den Wert in der dritten Zeile und zweiten Spalte der Matrix matrix.eins zu 5 zu ändern: matrix.eins[3,2] <- 5

`@instructions`
Herr Müller bittet Sie einen report.wochenverkaeufe für die Tochterfirma zu erstellen.

1. Ihre Aufgabe ist es eine Tabelle (Matrix) aus den Vektoren **sell.time und revenue.day** zu erstellen und der Variablen **report.wochenverkaeufe** zuzuordnen. Testen Sie, ob Sie es richtig gemacht haben mit der Ausgabe in der Console.

2.Sie haben den Report bei Herrn Müller abgeben. Er kommt auf Sie zu und entgegnet Ihnen, ob Ihnen aufgefallen sei, dass sich noch ein Zahlenfehler eingeschlichen hat. Kontrollieren Sie dies und ändern Ihn bitte ab.

- 2.1 Lassen Sie sich die Matrix report.wochenverkaeufe ausgeben.

- 2.2 Ändern Sie einen Fehler ab.

`@hint`


`@pre_exercise_code`
```{r}
#report.wochenverkaeufe <- matrix(1:18, ncol=6)
#sell.day <- c("Montag", "Dienstag", "Mittwoch", "Donnerstag", "Freitag", "Samstag")
sell.time <- c(8,18,8,8,9,6)
revenue.day <- c(2700, 3500, 4200, 4700, 5103, 3300)
average.byday <- c(2700/8, 3500/8, 4200/8, 4700/8, 5103/9, 3300/6)
```

`@sample_code`
```{r}
# report.wochenverkaeufe

# Ausgabe

# Änderung vornehmen

```

`@solution`
```{r}
#report.wochenverkaeufe <- matrix(1:18, ncol=6)
report.wochenverkaeufe <- rbind(sell.time, revenue.day)
# Ausgabe
print(report.wochenverkaeufe)
# Änderung vornehmen
report.wochenverkaeufe[1,2] <- 8
```

`@sct`
```{r}
ex() %>% check_code("report.wochenverkaeufe <- rbind(sell.time, revenue.day)", fixed=TRUE, missing_msg="Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau - Schauen Sie sich gern Ihre selbst erstellte Tabelle an!")
ex() %>% check_code("report.wochenverkaeufe[1,2] <- 8", fixed=TRUE, missing_msg="Sie haben den Fehler noch nicht richtig ausgebessert!") 
success_msg("Ja, genau - sonst wären falsche Umsatzzahlen an die Verkaufsniederlassung weitergegeben worden!")
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

- Struktur und Datentyp anzeigen lassen: **str()**
- Anzahl der Zeilen bzw. Spalten ausgeben lassen: **nrow() bzw. ncol()**

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
