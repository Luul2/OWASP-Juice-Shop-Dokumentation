## Deluxe Fraud

Im Juice Shop mit einem Benutzer anmelden und unter `http://localhost:3000/#/payment/deluxe` mit dem Inspektor den Pay-Button begutachten. Über den Inspector wird der Pay-Button untersucht. Um den Button freizuschalten, müssen die folgenden Elemente aus dem HTML-Code entfernt werden:
- *mat-mdc-button-disabled*
- *disabled="true"*

![JSBild](Bilder/deluxefraud.png)

Durch das Entfernen der entsprechenden Elemente lässt sich der Pay-Button nun betätigen. Die dabei erzeugte Anfrage wird mit Burp Suite abgefangen, um die an den Server übermittelten HTTP-Daten zu untersuchen. In Burp Suite den entsprechenden Request selektieren und diesen an den Repeater senden.

![JSBild](Bilder/deluxefraud1.png)

Im Request muss bei `paymentMode` anstatt `wallet` der Wert `paid` eingefügt werden.

![JSBild](Bilder/deluxefraud2.png)
