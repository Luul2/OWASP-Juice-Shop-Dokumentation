## Confidential Document

Mithilfe von gobuster und dem folgenden Befehl können versteckte Verzeichnisse herausgefunden werden:

    gobuster dir -u http://localhost:3000/ -w /usr/share/wordlists/dirb/common.txt --exclude-length 9903

![JSBild](Level1/Bilder/confidentialdocument1.png)

Bei dem Aufrufen des gefundenen Verzeichnisses http://localhost:3000/ftp/ wurden mehrere Dateien und Dokumente angezeigt: 

![JSBild](Level1/Bilder/confidentialdocument2.png)

Darunter befand sich unter anderem die Datei acquisitions.md, welches sich als vertrauliches Dokument herausstellte:

![JSBild](Level1/Bilder/confidentialdocument3.png)
