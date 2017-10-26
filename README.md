# Git Installationsanleitung

## Installation

### Debin/Ubuntu/Linux Mint
Das Programm git kann über die offiziellen Paketquellen bezogen werden. Dazu reicht der folgende Terminalbefehl.
```bash
sudo apt-get update && \
sudo apt-get dist-upgrade && \
sudo apt-get install git
```
Es lässt sich anschließend über das Terminal bedienen.

### MacOS
Für MacOS steht ein offizieller [Download](https://git-scm.com/download/mac) auf [git-scm.com](https://git-scm.com) bereit. Es findet wie unter Debian basierenden Betriebssystemen eine Integration in das Terminal statt.

### Windows
Für Windows können die Binärdateien wie bei MacOS von der offiziellen Website [heruntergeladen](https://git-scm.com/download/win) werden. Eine Integration in das Terminal (`cmd`) findet nicht statt. Stattdessen wird unter Windows das Programm git-bash installiert.

## Übung
Es besteht die Möglichkeit auf [github.io](https://try.github.io/levels/1/challenges/1) ein webbasiertes [Tutorial](https://try.github.io/levels/1/challenges/1) zu Thema git zu absolvieren. Alternativ dazu gibt es ein [Tutorial](https://git-scm.com/docs/gittutorial) auf [git-scm.com](https://git-scm.com).

## Repository klonen
Um ein Repository zu klonen finden Sie auf jeder Projektseite einen HTTPS und SSH Link. Den Download des Projekts mit SSH können Sie insofern durchführen, wenn Sie einen GitHub-Account haben und einen SSH-Public-Key in Ihren [Profileinstellungen](https://github.com/settings/keys) ihres Accounts hinterlegt haben. Durch den SSH-Key werden Sie beim Authentifizieren gegenüber der Seite [github.com](github.com) nicht nach ihrem Benutzernamen und ihrem Passwort gefragt.

Startet Sie die neu installierte git-bash unter Windows und navigieren Sie in ein beliebiges Verzeichnis mittels `cd` um dort das Repository herunter zu laden. Für Linux und Mac nutzer findet eine automatische Integration von git in das Terminal statt. Der Vorgang das git Repository zu klonen kann mittels `git clone <HTTPS- oder SSH-Link` gestartet werden. Sie sollten nun ein Verzeichnis haben, dass dem Namen des Projekts entspricht und den gleichen Inhalt wie wiederspielt wie dem aus dem Online-Repository.

## Weitere git Befehle
Wenn Sie nicht schon die gängigen git Befehle beherrschen, lernen Sie diese in Tutorien und Vorlesungen kennen. Die offizielle Dokumentation zu git finden Sie auf [git-scm.com](https://git-scm.com/docs). Es ist zu empfehlen sich folgende Grundbefehle für das Arbeiten mit git anzueignen.
* [git status](https://git-scm.com/docs/git-status)
* [git add](https://git-scm.com/docs/git-add)
* [git commit](https://git-scm.com/docs/git-commit)
* [git branch](https://git-scm.com/docs/git-branch)
* [git checkout](https://git-scm.com/docs/git-checkout)
* [git log](https://git-scm.com/docs/git-log)
* [git fetch](https://git-scm.com/docs/git-fetch)
* [git push](https://git-scm.com/docs/git-push)
* [git rebase](https://git-scm.com/docs/git-rebase)
* [git merge](https://git-scm.com/docs/git-merge)
* [git clone](https://git-scm.com/docs/git-clone)

Falls Sie die englische online Dokumentation stört und Sie nicht damit zurecht kommen, geht das Buch Git von Valentin Haenel und Julius Plenz auf den professionellen Umgang mit git ein - ISBN 978-3-95539-119-5.

## Videos
* Einrichten des repositories mit fh-trier als Downstream - [klick](./video/git_-_setup_upstream.mp4).
* Das lokale repository aktualisieren und Konflikte mit meld als mergetool beheben - [klick](git_-_rebase_and_merge_with_meld.mp4)

## Warum als git repository?
Dies dient als gute Grundlage den Studenten git als auch die Auszeichnugssprache [Markdown](https://guides.github.com/features/mastering-markdown/) näher zu bringen. Das Programm git kann als Revisionssystem übergreifend auch für andere Fächer wie beispielsweise Programmierung dienen und ermöglicht die Zusammenarbeit mit anderen Kommilitoten und Entwicklern weltweit.
Es ist zu empfehlen einen eigenen Account auf [github.com](https://github.com) zu erstellen, Projekte des Benutzers [FH-Trier](https://github.com/fh-trier) zu forken und seine eigenen Lösungen zu veröffentlichen. Verbesserungen von Projekten des Benutzers FH-Trier kann gerne per Merge-Request gestellt werden. Der Github-Account kann in späteren Bewerbungunterlagen als online Referenz angegeben werden um Unternehmen direkt vermitteln zu können, welche Kentnisse vorhanden sind. Dies sollte Sie von anderen Mitbewerbern hervorheben.

## Möglichkeiten
Während des Studiums werden Sie folgende Programmier- und Scriptspachen kennen lernen, die sich mit git versionieren lassen.

| Programmiersprache oder Skriptsprache | Dateiendung | Modul                                                           |
| ------------------------------------- | ----------- | --------------------------------------------------------------- |
| Java                                  | .java       | Programmierung 1 und 2, Objektorientierte Designpattern in Java |
| Latex                                 | .tex        | Seminar-, Bachelor- und Masterarbeiten                          |
| SQL-Dumpdateien                       | .sql        | Grundlagen Datenbanken, Datenbanken, Seminar Datenbanken        |
| R                                     | .r          | Data Mining                                                     |
| HTML(5)                               | .html       | Clientseitige Internettechnologien                              |
| PHP                                   | .php        | Serverseitige Internettechnologien                              |
| Bash                                  | .sh         | Linux 1 und 2                                                   |
| Perl                                  | .pl         | Linux 1 und 2                                                   |
| Ruby                                  | .rb         | Linux 1 und 2                                                   |

Neben diesen Programmiersprachen ist git in der Entwicklungsumgebung [IDE Intellij](https://www.jetbrains.com/idea/) integriert. Studenten erhalten über Nachweis ihres Studentenausweises eine Ultimate Version.

## Merge und Diff
Um einen Mergekonflikt oder ein diff per grafischen Oberfläche zu lösen oder zu betrachten empfiehlt sich das Programm [Meld](http://meldmerge.org/). Das Programm kann über die offizielle Seite für Windows Systeme [herunter geladen](https://download.gnome.org/binaries/win32/meld/3.16/Meld-3.16.2-win32.msi) werden. Bei Debian basierenden Systemen kann meld über offiziellen Paketquellen bezogen werden. Für Mac steht eine [Installationsanleitung](https://yousseb.github.io/meld/) auf github.io [bereit](https://yousseb.github.io/meld/).

Um allerdings git mitzuteilen, dass meld als Merge- bzw Difftool genutzt werden soll, sind einige Einstellungen notwendig.

```bash
# Für Debian, Mac, Ubuntu und Windows
git config --global user.name "Markus Pesch" # Ersetze den Namen
git config --global user.email "peschm@fh-trier.de" # Ersetze die E-Mail

git config --global diff.tool meld # Meld als Standard difftool einstellen
git config --global merge.tool meld # Meld als Standard mergetool einstellen

# Für Windows
# Den Programmpfad ggfs. anpassen
git config --global mergetool.meld.path"C:\Program Files (x86)\Meld\Meld.exe"

# Für Mac
cat << EOF >> ~/.gitconfig
	[diff]
  		tool = meld
	[difftool]
  		prompt = yes
	[difftool "meld"]
  		trustExitCode = true
  		cmd = open -W -a Meld --args \"$LOCAL\" \"$PWD/$REMOTE\"
	[merge]
  		tool = meld
	[mergetool]
  		prompt = yes
	[mergetool "meld"]
  		trustExitCode = true
  		cmd = open -W -a Meld --args --auto-merge \"$PWD/$LOCAL\" \"$PWD/$BASE\" \"$PWD/$REMOTE\" --output=\"$PWD/$MERGED\"
EOF

# Für Debian, Mac, Ubuntu und Windows
git config --global --list # Ausgabe der aktuellen git Einstellungen
git config --global --edit # Bearbeiten der aktuellen git Einstellungen

```




