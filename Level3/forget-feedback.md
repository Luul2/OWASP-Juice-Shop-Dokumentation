## Forged Feedback

Im Juice Shop mit einem Benutzer anmelden und unter `http://localhost:3000/#/contact` eine Bewertung abgeben. Dabei die Anfrage mit Burp Suite abfangen, um die an den Server übermittelten HTTP-Daten zu untersuchen.

![JSBild](Bilder/forgedfeedback.png)

In Burp Suite den entsprechenden Request selektieren und bei diesem den Wert für die `User-ID` abändern.

![JSBild](Bilder/forgedfeedback1.png)
