## Admin Registration

Im Juice Shop einen neuen Benutzer unter der `http://localhost:3000/#/register` anlegen und registrieren. Dabei die Anfrage mit Burp Suite abfangen, um die an den Server übermittelten HTTP-Daten zu untersuchen.

![JSBild](Bilder/adminregistration.png)

In Burp Suite den entsprechenden Request selektieren und diesen an den Repeater senden.

![JSBild](Bilder/adminregistration1.png)

Im Repeater kann die zugehörige Response des Servers eingesehen werden. Dabei ist zu erkennen, dass dem Parameter `role` der Wert `customer` zugewiesen ist.

![JSBild](Bilder/adminregistration2.png)

Im Request muss demnach `"role":"admin"` eingefügt werden:

![JSBild](Bilder/adminregistration3.png)

Anschließend wird der modifizierte Request an den Server gesendet.
