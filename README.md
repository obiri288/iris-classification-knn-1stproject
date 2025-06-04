# iris-classification-knn-1stproject
# Irisblüten-Klassifizierung mit K-Nearest Neighbors (KNN)

## Inhaltsverzeichnis
1.  [Beschreibung](#beschreibung)
2.  [Datensatz](#datensatz)
3.  [Verwendete Technologien](#verwendete-technologien)
4.  [Setup und Ausführung](#setup-und-ausführung)
5.  [Projektstruktur](#projektstruktur)
6.  [Ergebnisse](#ergebnisse)
7.  [Lernziele](#lernziele)
8.  [Autor](#autor)
9.  [Lizenz](#lizenz)

---

## Beschreibung

Dieses Projekt demonstriert eine grundlegende Klassifizierungsaufgabe im Bereich des maschinellen Lernens: die Unterscheidung verschiedener Arten von Irisblüten (Setosa, Versicolor, Virginica) anhand ihrer morphologischen Merkmale (Kelchblatt- und Blütenblattlänge sowie -breite). Hierfür wird der K-Nearest Neighbors (KNN)-Algorithmus eingesetzt.

Der gesamte Prozess, von der Datenbeschaffung über das Modelltraining und die Evaluierung bis hin zur Visualisierung der Ergebnisse, ist im beigefügten Python-Code (Jupyter Notebook) dokumentiert. Ziel war es, ein klares Verständnis für die einzelnen Schritte eines typischen Machine-Learning-Workflows zu entwickeln.

---

## Datensatz

Es wurde der klassische **Iris-Datensatz** verwendet, der direkt über die `scikit-learn`-Bibliothek geladen wird.
* **Anzahl der Beobachtungen:** 150
* **Anzahl der Merkmale:** 4
    * Kelchblattlänge (cm)
    * Kelchblattbreite (cm)
    * Blütenblattlänge (cm)
    * Blütenblattbreite (cm)
* **Zielklassen:** 3 (Iris Setosa, Iris Versicolor, Iris Virginica), im Code numerisch als 0, 1, 2 repräsentiert.

---

## Verwendete Technologien

* **Programmiersprache:** Python 3.x
* **Kernbibliotheken für Machine Learning & Datenverarbeitung:**
    * `scikit-learn`: Für den KNN-Algorithmus, das Laden des Iris-Datensatzes, die Aufteilung der Daten (`train_test_split`) und diverse Evaluierungsmetriken (`accuracy_score`, `classification_report`, `confusion_matrix`).
    * `pandas`: Zur Handhabung der Daten in tabellarischer Form (DataFrames).
    * `numpy`: Für effiziente numerische Berechnungen.
* **Visualisierungsbibliotheken:**
    * `matplotlib.pyplot`: Zur Erstellung von Diagrammen und Plots.
    * `seaborn`: Für statistische Datenvisualisierung, hier insbesondere für die Heatmap der Konfusionsmatrix und den Scatterplot der Entscheidungsgrenzen.
    * `matplotlib.colors.ListedColormap`: Zum Definieren eigener Farbschemata für die Plots.
* **Entwicklungsumgebung:** Der Code ist als Jupyter Notebook strukturiert und wurde primär für die Ausführung in Google Colaboratory konzipiert, kann aber auch in anderen Jupyter-Umgebungen ausgeführt werden.

---

## Setup und Ausführung


1.  **Notebook öffnen und ausführen:**
    * Öffne die Datei 
    * Führe alle Zellen des Notebooks nacheinander aus. Der bereitgestellte Python-Code enthält alle notwendigen Importe und Schritte. Die benötigten Bibliotheken sind Standard und sollten in den meisten Python-ML-Umgebungen verfügbar sein oder können via `pip install scikit-learn pandas numpy matplotlib seaborn` installiert werden.



---

## Projektstruktur

---

## Ergebnisse

Der im Notebook trainierte K-Nearest Neighbors (KNN) Klassifikator (mit `n_neighbors=3`) erzielt auf dem Testdatensatz folgende Leistung:

* **Genauigkeit (Accuracy):** **100%**


* **Klassifikationsbericht:** Das Notebook generiert einen detaillierten Bericht mit Precision, Recall und F1-Score für jede der drei Iris-Arten.
* **Konfusionsmatrix:** Eine visualisierte Konfusionsmatrix zeigt die Anzahl der korrekten und inkorrekten Vorhersagen für jede Klasse.
* **Visualisierung der Entscheidungsgrenzen:** Ein Plot illustriert, wie das KNN-Modell den zweidimensionalen Merkmalsraum (basierend auf Blütenblattlänge und -breite) aufteilt, um die verschiedenen Iris-Arten zu klassifizieren.


## Lernziele

Dieses Projekt diente der praktischen Anwendung und dem Verständnis folgender grundlegender Konzepte des maschinellen Lernens:
* Der End-to-End-Workflow eines Klassifikationsprojekts.
* Laden, Untersuchen und Vorbereiten von Daten für das maschinelle Lernen.
* Die Notwendigkeit und Implementierung der Aufteilung von Daten in Trainings- und Testsets zur validen Modellevaluierung.
* Die Funktionsweise, das Training und die Anwendung des K-Nearest Neighbors (KNN)-Algorithmus.
* Interpretation verschiedener Metriken zur Leistungsbewertung eines Klassifikationsmodells (Genauigkeit, Precision, Recall, F1-Score, Konfusionsmatrix).
* Die Bedeutung und Erstellung von Visualisierungen (wie Entscheidungsgrenzen) zur besseren Interpretation des Modellverhaltens.

---

## Autor

* **obiri288**
* GitHub: `https://github.com/obiri288`


---

## Lizenz

Dieses Projekt steht unter der **MIT Lizenz**.


