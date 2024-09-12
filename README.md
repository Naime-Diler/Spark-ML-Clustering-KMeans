# **Spark Machine Learning - Clustering: K-Means**

In diesem Projekt wird die Clustering-Methode K-Means auf einen Churn-Datensatz angewendet, um natürliche Gruppierungen der Daten zu identifizieren. K-Means ist ein beliebter Algorithmus des unüberwachten Lernens, bei dem keine Zielvariable vorgegeben ist. Die wesentlichen Schritte des Projekts sind:

**Datenvorbereitung**: Der Datensatz wird aus einer CSV-Datei geladen und in einem DataFrame gespeichert. Die Datentypen werden überprüft, und der Datensatz wird im Speicher gehalten, um die Verarbeitung zu beschleunigen.

**Datenverarbeitung**: Kategorische und numerische Merkmale werden identifiziert. Kategorische Spalten werden bereinigt und für die One-Hot-Codierung vorbereitet. Für die Kategorisierung werden StringIndexer und OneHotEncoder verwendet.

**Modelltraining**: Ein K-Means-Clustering-Modell wird innerhalb einer Spark-Pipeline trainiert. Die Pipeline umfasst die Schritte der Datenumwandlung, Feature-Extraktion und Skalierung.

**Evaluation**: Die Modellleistung wird mit dem ClusteringEvaluator bewertet, um den besten Wert für die Anzahl der Cluster (k) zu bestimmen.

**Ergebnisse**: Die Clusterzuweisungen zeigen, wie die Datenpunkte gruppiert wurden. Ein Vergleich der Clusterzuweisungen mit den tatsächlichen Klassenzuweisungen ist möglich, jedoch nicht immer zu erwarten.

Dieses Projekt veranschaulicht, wie Spark ML für das Clustering von Daten verwendet wird, um Muster und Gruppen innerhalb der Daten zu erkennen.
