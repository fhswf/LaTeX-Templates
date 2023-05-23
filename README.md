# LaTeX und Markdown Templates

Vorlagen für Abschlussarbeiten und schriftliche Ausarbeitungen.

## LaTeX

Zum Kompilieren eines Dokuments wird die TeX-Distribution *TeX Live* benötigt.

**Windows**

Für Windows existiert ein Installer: [www.tug.org/texlive](https://www.tug.org/texlive/)

Als Editor für das Bearbeiten und Kompilieren von LaTeX-Dokumenten ist *TeXstudio* sehr zu empfehlen: [www.texstudio.org](https://www.texstudio.org/)

Nach der Installation von TeXstudio muss noch *Biber* als Bibliographieprogramm ausgewählt werden: *Optionen* > *TeXstudio konfigurieren* > *Erzeugen* > *Standard Bibliographieprogramm: Biber*

**Ubuntu**

Installation über die Paketverwaltung in der Shell:

    sudo apt-get install texlive texlive-lang-german texlive-latex-extra biber

Installation des Editors *TeXstudio*:

    sudo apt-get install texstudio

Wie oben beschrieben muss anschließend *Biber* konfiguriert werden.

## Markdown

Es wird dieselbe LaTeX-Installation vorausgesetzt wie oben beschrieben!

Zusätzlich muss beim Kompilieren die Option `-shell-escape` verwendet werden. Beim Kompilieren in der Kommandozeile wird *pdflatex* dazu mit der genannten Option aufgerufen: `pdflatex -shell-escape Abschlussarbeit`. Bei der Verwendung eines Editors muss die Option über das Einstellungsmenü in die Konfiguration von *pdflatex* eingetragen werden.

Da Markdown im Vergleich zu LaTeX nur über beschränkte Gestaltungsmittel verfügt, besteht die Möglichkeit, im Markdown-Dokument auch LaTeX-Makros zu verwenden. Dazu muss im Hauptdokument (`Abschlussarbeit.tex`) die Option `hybrid` des Pakets *markdown* aktiviert werden ([Dokumentation](https://www.ctan.org/pkg/markdown) des Pakets auf CTAN, [Tutorial](https://www.overleaf.com/learn/how-to/Writing_Markdown_in_LaTeX_Documents) auf Overleaf).
