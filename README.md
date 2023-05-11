# LaTeX und Markdown Templates

Vorlagen für Abschlussarbeiten und schriftliche Ausarbeitungen.

## LaTeX

Zum Kompilieren eines Dokuments wird die TeX-Distribution *TeX Live* benötigt.

**Windows**

Für Windows existiert ein Installer: [www.tug.org/texlive](https://www.tug.org/texlive/)

In der Installation ist der Editor *TeXworks* enthalten, mit dem LaTeX-Dokumente editiert und kompiliert werden können.

**Ubuntu**

Installation über die Paketverwaltung in der Shell:

    sudo apt-get install texlive texlive-lang-german texlive-latex-extra biber

Installation des Editors *Kile* (es existieren auch andere Editoren):

    sudo apt-get install kile

## Markdown

Es wird dieselbe LaTeX-Installation vorausgesetzt wie oben beschrieben!

Zusätzlich muss beim Kompilieren die Option `-shell-escape` verwendet werden. Beim Kompilieren in der Kommandozeile wird *pdflatex* dazu mit der genannten Option aufgerufen: `pdflatex -shell-escape Abschlussarbeit.tex`. Bei der Verwendung eines Editors muss die Option über das Einstellungsmenü in die Konfiguration von *pdflatex* eingetragen werden.

Da Markdown im Vergleich zu LaTeX nur über beschränkte Gestaltungsmittel verfügt, besteht die Möglichkeit, im Markdown-Dokument auch LaTeX-Makros zu verwenden. Dazu muss im Hauptdokument (`Abschlussarbeit.tex`) die Option `hybrid` des Pakets *markdown* aktiviert werden ([Dokumentation](https://www.ctan.org/pkg/markdown) des Pakets auf CTAN, [Tutorial](https://www.overleaf.com/learn/how-to/Writing_Markdown_in_LaTeX_Documents) auf Overleaf).
