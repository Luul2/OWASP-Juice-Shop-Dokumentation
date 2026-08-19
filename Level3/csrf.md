## CSFR

Im Juice Shop mit einem Benutzer anmelden und unter `http://localhost:3000/profile` den Benutzernamen ändern. Dabei die Anfrage mit Burp Suite abfangen, um die an den Server übermittelten HTTP-Daten zu untersuchen.

![JSBild](Bilder/csrf.png)

In Burp Suite den entsprechenden Request selektieren. Dabei ist zu erkennen, dass der neue Benutzername über den Parameter `username` an den Server übermittelt wird.

![JSBild](Bilder/csrf1.png)

Anschließend eine HTML-Seite erstellen, die den Parameter `username` mit dem Wert `HackerName` an den Juice Shop übermittelt.

![JSBild](Bilder/csrf2.png)

Beim Öffnen der HTML-Seite wird ein Button mit der Beschriftung `Absenden` angezeigt. 

![JSBild](Bilder/csrf3.png)

Durch das Betätigen des Buttons wird die vorbereitete Anfrage an den Juice Shop gesendet und der Benutzername entsprechend geändert.

![JSBild](Bilder/csrf4.png)
