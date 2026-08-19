## Payback Time

Im Juice Shop ein oder mehrere Produkte zum Warenkorb hinzufügen. Zu  `http://localhost:3000/basket` navigieren und die Menge des Produktes erhöhen. Dabei die Anfrage mit Burp Suite abfangen, um die an den Server übermittelten HTTP-Daten zu untersuchen.

![JSBild](Bilder/paybacktime1.png)

![JSBild](Bilder/paybacktime2.png)

In Burp Suite den entsprechenden Request selektieren und bei diesem den Wert für `quantity` von 6 auf -12345 abändern.

![JSBild](Bilder/paybacktime3.png)

Nach dem Absenden des modifizierten Requests erscheint ein negativer Gesamtbetrag im Warenkorb.

![JSBild](Bilder/paybacktime4.png)
