# EA 10 - Instance Based Algs KNN Exercise
### Data Science SS 21
### Christian Kitte 

### Exercise 1 von 2: Implementierung eines eigenen KNN Algorithmus für maximal zwei Dimensionen

Für die Umsetzug dieser Aufgabe nutze ich den um ein Klassenmerkmal erweiterten Datensatz aus der Regressionsübung.

#### Fiktiver Kontext:
An freien Mitarbeitern werden Aufträge vergeben, welche nach vorheriger Absprache von diesen zu erledigen sind. Es ist normal, dass es eine Reihe von Gründen gibt, warum diese nicht erfolgreich sind. Nicht immer sind diese von den Mitarbeitern zu vertreten. Ein Auftrag wurde erfolgreich erledigt, sofern er fristgerecht und korrekt zur weiteren Verwendung vorliegt. Um hier nach möglichen Zusammenhängen zu suchen, wurde die Zahl der zugeteilten sowie der Erledigten Aufträge notiert. Hierbei können natürlich nur Aufträge einer vergleichbaren Art zusammen ausgewertet werden (beispielsweise nur im gleichen Bereich oder gleicher Zielgruppe).

Die [**hier vorliegende CSV Datei Auftraege.csv**](https://github.com/ChristianKitte/HelloKNN/blob/main/Auftraege.csv) enthält die fiktive Anzahl von vergebenen Aufträgen und die Anzahl der hiervon erfolgreich durchgeführten. Hierbei wurden die Zahlen bereinigt, so dass nur die tatsächlich zu realisierenden Aufträge Berücksichtigung finden. Weiter wurden die Anzahl der Aufträge durch die Anzahl der erfolgreichen Aufträge dividiert und anhand des Wertes eine Klassifizierung vorgenommen. Die Frage, inwieweit dies Verfahren tatsächlich sinnvoll ist, soll hier nicht näher betrachtet werden.

Es ergeben sich folgende Klassen:

* 0 unbestimmt
* 1 Top
* 2 Best
* 3 Score
* 4 Underscore

#### Ergebnis:
Die komplette und ausführliche Lösung dieser Aufgabenstellung findet sich in diesem [**Notebook**](https://github.com/ChristianKitte/HelloKNN/blob/main/KNN_Algorithmus.ipynb). Insbesondere wurde die Funktionalität für die Normalisierung zwei dimensionaler Daten sowie der Entfernungsberechnung für diesen Raum "von Hand" implementiert. Ebenso die Logik für die Verarbeitung der Daten, der Auszählung der k-Klassen sowie die Auswahl des besten Ergebnisses. 

An vielen Stellen enthält der Code zusätzlichen Quelltext, um die eigenen Methoden zu validieren respektive zu vergleichen. Hier kam die Bibliothek SciKit Learn (Sklearn) und deren Methoden zum Einsatz.

Ein abschließender Test zeigte, dass der so implementierte Algorithmus mit k=10 ein gutes Ergebnis für die fiktiven Daten liefert. Selbstredend wäre eine "professionelle" Umsetzung vom Code her wesentlich kompakter und übersichtlicher. Dafür kann das Notebook eine Basis für Versuche darstellen.

### Exercise 2 von 2: Klassifizierung mit Hilfe von KNN

You are walking in the forrest and see an iris and measure: 4.8,2.5,5.3,2.4.
Is this an Iris Virginica or not? 

Als Basis zur Bearbeitung dient das berühmte [**Iris flower data set**](https://en.wikipedia.org/wiki/Iris_flower_data_set).

#### Ergebnis:

Die komplette und ausführliche Lösung dieser Aufgabenstellung findet sich in diesem [**Notebook**](https://github.com/ChristianKitte/HelloKNN/blob/main/KNN_sklearn.ipynb). Bei der Bearbeitung wurde die Bibliothek SciKit Learn (Sklearn) und deren Methoden eingesetzt, welche die Umsetzung und Anwendung des Verfahrens sehr vereinfachen. Besonders sind hier die Methoden zur Normalisierung und dem eigentlichen KNN Algorithmus zu nennen.

Abschließend komme ich zu dem Ergebnis, dass es sich bei er Blume um eine Iris Virginica handelt! Das Ergebnis der vorherigen [**Übung zur Regression**](https://github.com/ChristianKitte/HelloRegression) wird hierdurch bestätigt.

#### Anmerkung:

Ein großer Teil des im Notebook für die Aufgaben verwendeten Codes dient lediglich der Verdeutlichung, Visualisierung und sonstiger Ausgaben und kann grundsätzlich entfallen. Es ist hierbei erstaunlich, wie hilfreich eine Bibliothek wie sklearn sein kann. Dies macht Lust, es in der eigenen Praxis mit einzubringen. Wer sich primär nur für die abschließenden Ergebnisse interessiert, findet diese am Ende der Notebooks :).

