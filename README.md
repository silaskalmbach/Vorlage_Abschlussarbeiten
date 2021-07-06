# LaTeX @ILEK
Diese Vorlage dient als grober Leitfaden zu Erstellung der Abschlussarbeit. Die Formatierung ist somit nicht zwingend umzusetzen.

Die Formatierung des Deckblattes sollte, soweit möglich, unverändert bleiben. 

Von der Gliederung der Arbeit kann abgewichen werden, solang dieses sinnig begründbar ist.

# LaTeX Grundlagen
Um mit LaTeX zu Arbeiten, wird einerseits ein Editor und andererseits eine LaTeX-Distribution benötigt. Der Editor dient hierbei zur Eingabe des LaTeX-Code, die LaTeX-Distribution übersetzt den Code in ein Dokument. 

Beispielsweise kann eine Kombination der folgende Programme verwendet werden:

1. MiKTeX https://miktex.org/download (LaTeX-Distribution)

1. TeXstudio https://www.texstudio.org/ (Editor)

Alternativ besteht auch die Möglichkeit Online-Dienste zu benutzen, welche mögliche Schwierigkeiten bei der Einrichtung der oben genannten Lösung umgehen. Diese vereinen Editor und LaTeX-Distribution.

1. Overleaf https://de.overleaf.com/

Für eine problemlose Kompilierung des \LaTeX-Dokumentes ist es notwendig, einige Einstellungen in den Editor zu übernehmen.

1. Als Standardcompiler wird LuaLaTeX oder PdfLaTeX empfohlen

1. Als Standard Bibliographieprogramm sollte Biber ausgewählt werden

# Hinweis zur Abgabe

## Gedrucktes Exemplar
In der Regel sollten insgesamt zwei Examplare an das ILEK ausgehändigt werden. Für den Druck gelten die folgenden Empfehlungen:

- Dickeres Papier (z.B. 100-120 g/m²)
- Softcover mit Kaltleimbindundung
- Für den Einband sollte der [Umschlag](#01_frontcover) verwendet werden 

Die Auswahl eines ein- oder doppelseitigen Druckes richtet sich nach der Seitenzahl. Bis ca. 50 Seiten wird ein einseitiger Druck empfohlen, darüber hinaus ein doppelseitiger.

Wichtig bei der Auswahl eines ein- oder doppelseitigen Druckes ist das LaTeX-Dokument entsprechend anzupassen. Dadurch werden die Seitenränder und Seitenzahl korrekt ausgerichtet.

- Doppelseitiger Druck: In der main.tex-Datei die Option `<twoside>` auswählen
- Einseitiger Druck: In der main.tex-Datei die Option `<twoside>` auskommentieren (Standarteinstellung)

Mit diesen Informationen einfach an das Kopiergeschäft herantreten, diese wissen meist was zu tun ist.

## Digitales Exemplar (PDF)
Hierfür in der main.tex-Datei die Option `<twoside>` auskommentieren (Standarteinstellung).

Bitte die Arbeit in digitaler Form auf einer CD speichern und einem der gedruckten Exemplare beilegen. Die CD sollte ebenso das LaTeX-Dokument, alle Abbildung und die während der Arbeit erstellten Berechnungen (bswp. in Form von Excel-Tabellen, Programmcode oder FE-Berechnungen ohne Ergebnisse) enthalten.

# Aufbau des Ordners
Der Aufbau des Ordners ist an der Struktur der Abschlussarbeit orientiert. 

Die Ordner und Dateien in denen nicht zwingend Anpassungen vorgenommen werden müssen sind im folgenden gekennzeichnet. Natürlich können diese dennoch angepasst werden.

Hinweise zu den jeweiligen Abschnitten und dem dazugehörigen LaTeX-Code sind auch in den Kommentaren im Code zu finden!

## Jahr_Nachname_Titel_der_Arbeit.tex
Diese Datei ist der Startpunkt des Dokumentes. Hier werden alle im folgenden aufgelisteten Abschnitte referenziert. Um das Gesamtdokument zu erstellen muss diese Datei kompiliert werden.

## Frontcover.tex
Referenziert auf den Einband der Arbeit. Um den Einband zu erstellen muss diese Datei kompiliert werden.
## _A_frontmatter
Die Titelei (englisch front matter) bezeichnet die Seiten, die dem eigentlichen Inhalt vorangestellt sind.

### 01_frontcover
Enthält den Einband bzw. das Deckblatt der Arbeit. Keine Anpassungen notwendig.

Wichtig: Die Datei coverEnvelope.pdf dient enthält den Umschlag zur Einreichung beim Druck der Arbeit im Kopiergeschäft. Am besten im Vorraus mit dem Kopiergeschäft abstimmen wie dick die Arbeit wird, sodass der Rücken des Umschlages die richtige Breite hat. Diese hängt ab von der Anzahl der Seiten, der Dicke des Papiers sowie ob ein- oder doppelseitig gedruckt wird.

Die Breite des Einbandes wird in den [Variablen](#variables.tex) eingestellt.
### 02_cover
Enthält das Titelblatt der Arbeit. 

### 03_copyright.tex
Enthält die eidesstattliche Erklärung zur eigenen Anfertigung der Arbeit. Keine Anpassungen notwendig.

### 04_acknowledgements.tex
Enthält die Danksagung. 

### 05_assignment
Kann optional auch weggelassen werden. Enthält ein PDF mit der Aufgabenstellung.

### 06_abstract
Enthält die englische und deutsche Kurzfassung der Arbeit.

### 07_nomenclature
Enthält Symbole und Abkürzungen die in der Arbeit verwendet werden. Keine Anpassungen notwendig.

Alternativ kann dieser Abschnitt auch ins Backmatter vor das Abbildungsverzeichnis eingefügt werden.

## _B__mainmatter
Ab hier beginnt der Hauptteil der Abschlussarbeit. Der Aufbau dieses Ordner kann beliebig angepasst werden.

### 01_examples.tex
Die einzelnen Dateien enthalten Beispiele für Formatierungen von Tabellen, Bildern etc. und dienen als Orientierung.

### images
Die verwendeten Abbildungen können in diesem Ordner abgelegt werden. Auch der Aufbau dieses Ordner kann beliebig angepasst werden.

## _C_appendix
Ab hier beginnt der Anhang der Abschlussarbeit. Auch hier gilt das der Aufbau dieses Ordner beliebig angepasst werden kann.

Der Vorschlag für den Aufbau orientiert sich an II_mainmatter.

## _D_backmatter
Ab hier beginnet der Schlussteil der Arbeit.

### references.tex
Enthält das Abbildungs-, Tabellen- und Literaturverzeichnis. 

### literatur.bib

Enthält die Daten für das Literaturverzeichnis der Arbeit. Keine Anpassungen notwendig.

Empfohlen wird die Verwaltung und Anfertigung des Literaturverzeichnisses mit den folgenden Programmen. Es bietet sich an bereits zu beginn der Abschlussarbeit alle Quellen mit den genannten Programmen zu verwalten

1. Citavi https://www.citavi.com/de

1. Zotero https://www.zotero.org/

## _E_ressources
Enthält notwendige Einstellungen und Dateien für LaTex.

### preambel.tex
In der Präambel werden alle für das gesamte Dokument gültigen Formatierungseinstellungen getroffen sowie zusätzlich benötigte Pakete geladen. Keine Anpassungen notwendig.

### variables.tex
Enthält alle wichtigen Angaben (Titel, Betreuer, Jahr ..) zur Arbeit. Diese müssen entsprechend angepasst werden sodass Einband und Titelblatt mit den richtigen Informationen erstellt werden.

### fonts
Enthält die Schriftart der Universität Stuttgart. Aufgrund der Lizenzierung der Schrift dürfen wir die dafür notwendigen Dateien nicht über GitHub zu Verfügung stellen. 

Daher entweder den Betreuer der Arbeit nach den entsprechenden Dateien fragen oder alternativ Arial verwenden (automatisch eingestellt wenn die Schriftart Univers for UniS nicht gefunden wird).

Die Schriftarten der Universität Stuttgart müssen wie folgt benannt werden:

- UniversforUniS45LtObl-Rg
- UniversforUniS55Rm-Regular
- UniversforUniS65Bd-Regular

### tikz
Durch Tikz Kompilierte Grafiken. Keine Anpassungen notwendig.
