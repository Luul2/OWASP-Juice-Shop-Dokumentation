## GDPR Data Erasure

Im Juice Shop auf der Anmeldeseite `http://localhost:3000/#/login` als E-Mail lediglich ' angeben und als Passwort irgendetwas wählen. Die dabei erzeugte Anfrage mit Burp Suite abfangen, um die an den Server übermittelten HTTP-Daten zu untersuchen. 

![JSBild](Bilder/gdpr.png)

Anschließend in Burp Suite den entsprechenden Request selektieren und untersuchen. Die vom SQL-Server ausgegebene Fehlermeldung gibt Hinweise auf die Struktur der verwendeten SQL-Abfrage, wobei die Anwendung das Feld `deletedAt` überprüft.

![JSBild](Bilder/gdpr1.png)

Durch die Eingabe von `' OR DeletedAt IS NOT NULL --` in das E-Mail-Feld und eines beliebigen Passworts kann die SQL-Abfrage manipuliert werden. Dadurch wird die Anmeldung mit dem gelöschten Benutzerkonto von Chris ermöglicht.

![JSBild](Bilder/gdpr2.png)
