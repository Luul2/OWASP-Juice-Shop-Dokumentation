## Manipulate Basket

Im Juice Shop mit einem Benutzer anmelden und unter `http://localhost:3000/` Produkte zu dem Warenkorb hinzufügen und in den Warenkorb gehen. Dabei den HTTP-Verkehr mit Burp Suite abfangen, um die an den Server übermittelten Daten zu untersuchen.

![JSBild](Bilder/manipulatebasket.png)

In Burp Suite den entsprechenden Request selektieren. 

![JSBild](Bilder/manipulatebasket1.png)

Diesen an den Repeater übermitteln und die BasketId duplizieren, jedoch mit einer anderen Nummer.

![JSBild](Bilder/manipulatebasket2.png)

![JSBild](Bilder/manipulatebasket3.png)

Nach dem Absenden des modifizierten Requests wurden die ausgewählten Produkte erfolgreich dem Warenkorb des Benutzers mit der ID `2` hinzugefügt.
