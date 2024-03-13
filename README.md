
# Analyse von Immobilienverkaufsdaten der Stadt Milwaukee

Dieses Projekt konzentriert sich auf die Analyse von Immobilienverkaufsdaten, um Muster und Einflussfaktoren auf den Verkaufspreis von Immobilien in Milwaukee zu identifizieren. Das Hauptziel ist es, ein präzises Prognosemodell für die Vorhersage von Verkaufspreisen zu entwickeln, das den Verkaufspreis basierend auf verschiedenen Eigenschaften der Immobilie möglichst valide vorhersagen kann.

## Umgebung

- **Entwicklungsumgebung:** Jupyter Notebook
- **Python-Version:** 3.11
- **Benötigte Libraries:** pandas, sklearn, shap, mlflow, dotenv 

## Datensatz

Der Datensatz umfasst verschiedene Merkmale von Immobilien, einschließlich des Typs, des Bezirks, des Baustils, des Baujahrs, der Wohnfläche, der Anzahl der Badezimmer, der Grundstücksgröße, des Verkaufsdatums und des Verkaufspreises.

**Quelle des Datensatzes:** [Milwaukee Data Portal](https://data.milwaukee.gov/dataset/7a8b81f6-d750-4f62-aee8-30ffce1c64ce/resource/f083631f-e34e-4ad6-aba1-d6d7dd265170/download)


## Analyseprozess
Aufbauend auf den Lernunterlagen aus dem Modul ADSC21 Applied Data Science II, Sebastian Seck (DBU) 

1. **Daten einlesen**: Der erste Schritt beinhaltet das Einlesen der Daten aus einer CSV-Datei. Für das zentrale Ergebnisnotebook namens "Main_final_Noebook" wird der Datensatz subset.wohnraum_clean verwendet. Dabei werden die schon vorverarbeiteten Daten verwendet, die sich nur mehr auf den Bereich Wohnraum also Wohnimmobilien konzentrieren. 
2. **Vorverarbeitung**: In diesem Schritt werden die Daten aufbereitet, neue Features wurden entwickelt wobei fehlende Werte ersetzt und kategorische Variablen in numerische umgewandelt werden.
3. **Aufteilung in Trainings- und Testdaten**: Die Daten werden in ein Trainings- und ein Testset aufgeteilt.
4. **Modellentwicklung**: Verschiedene Modelle werden trainiert und evaluiert, um das Modell mit der besten Vorhersagegenauigkeit zu identifizieren.
5. **Modellvergleich und -auswahl**: Mehrere Modelle werden verglichen, um das effektivste auszuwählen.
6. **Hyperparametertuning**: Durch Grid Search wird das Modell weiter optimiert.
7. **Modellbewertung**: Die Leistung des finalen Modells wird anhand verschiedener Metriken bewertet. In der Hauptdatei namens "Main_final_Noebook" werden alle Modelle nochnmals mit dem finalen und in mehreren Iterationen optimierten Breinigungen verwendet. 

## Ergebnisse

Die Analyse zeigt, dass das Gradient Boosting Regressor-Modell mit spezifischen Hyperparametern die besten Ergebnisse liefert. Die Evaluation erfolgte auf Basis des R²-Wertes, des mittleren absoluten Fehlers (MAE).

## Verwendung

Um das "Main_final_Noebook" zu verwenden, müssen jedenfalls folgende neben der Aktivierung der ads-ml-full-Python 3.11.8. Umgegbung vorgesehenen Requirements installiert werden und die Zellen sind von oben nach unten auszuführen.


