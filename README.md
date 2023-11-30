# LaTeX-Vorlagen

Vorlagen für Abschlussarbeiten und schriftliche Ausarbeitungen.

## LaTeX

Zum Kompilieren eines Dokuments wird die TeX-Distribution *TeX Live* benötigt. Als Editor für das Bearbeiten und Kompilieren von Dokumenten ist *TeXstudio* zu empfehlen.

**Windows**

Für Windows gibt es Installer:

- TeX Live: [www.tug.org/texlive](https://www.tug.org/texlive/)
- TeXstudio: [www.texstudio.org](https://www.texstudio.org/)

Nach der Installation von TeXstudio muss *Biber* als Bibliographieprogramm ausgewählt werden:  
*Optionen* > *TeXstudio konfigurieren* > *Erzeugen* > *Standard Bibliographieprogramm: Biber*

**macOS**

Auf dem Mac wird TeX Live unter dem Namen *MacTeX* angeboten: [www.tug.org/mactex](https://www.tug.org/mactex/)

Die Entwicklungsumgebung *TeXShop* ist bereits in MacTeX enthalten. Auf Wunsch kann TeXstudio ([www.texstudio.org](https://www.texstudio.org/)) nachinstalliert werden.

**Ubuntu**

Installation von TeX Live über die Paketverwaltung in der Shell:

    sudo apt-get install texlive texlive-lang-german texlive-latex-extra biber

Installation des Editors TeXstudio:

    sudo apt-get install texstudio

Wie oben beschrieben muss anschließend Biber konfiguriert werden.

## Markdown

Da Markdown im Vergleich zu LaTeX nur über sehr beschränkte Gestaltungsmöglichkeiten verfügt, ist es für längere Arbeiten eher ungeeignet. Besonders für Abschlussarbeiten empfiehlt sich die Einarbeitung in LaTeX. Ein Einstiegstutorial gibt es zum Beispiel hier: [overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes)

**Konfiguration**

Es wird dieselbe LaTeX-Installation vorausgesetzt wie oben beschrieben!

Zusätzlich muss beim Kompilieren die Option `-shell-escape` verwendet werden. Beim Kompilieren in der Kommandozeile wird *pdflatex* dazu mit der genannten Option aufgerufen: `pdflatex -shell-escape Abschlussarbeit`. Bei der Verwendung eines Editors muss die Option über das Einstellungsmenü in die Konfiguration von *pdflatex* eingetragen werden.

Es besteht die Möglichkeit, im Markdown-Dokument auch LaTeX-Makros zu verwenden. Dazu muss im Hauptdokument die Option `hybrid` des Pakets *markdown* aktiviert werden ([Dokumentation](https://www.ctan.org/pkg/markdown) des Pakets auf CTAN, [Tutorial](https://www.overleaf.com/learn/how-to/Writing_Markdown_in_LaTeX_Documents) auf Overleaf).
