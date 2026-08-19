## Forged Review

Im Juice Shop mit einem Benutzer anmelden und unter `http://localhost:3000/` eine Bewertung unter einem Produkt abgeben. Dabei die Anfrage mit Burp Suite abfangen, um die an den Server übermittelten HTTP-Daten zu untersuchen.

![JSBild](Bilder/forgedreview.png)

In Burp Suite den entsprechenden Request selektieren und bei diesem den Wert für den `author` auf einen anderen Benutzer abändern.

![JSBild](Bilder/forgedreview1.png)

![JSBild](Bilder/forgedreview2.png)

Nach dem Absenden des modifizierten Requests wird die Bewertung unter dem Namen des angegebenen Benutzers veröffentlicht.

![JSBild](Bilder/forgedreview3.png)
