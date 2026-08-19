## CAPTCHA Bypass

Im Juice Shop mit einem Benutzer anmelden und unter `http://localhost:3000/#/contact` eine Bewertung abgeben. Die dabei erzeugte Anfrage mit Burp Suite abfangen, um die an den Server übermittelten HTTP-Daten zu untersuchen. 

![JSBild](Bilder/captcha.png)

In Burp Suite den entsprechenden Request selektieren und diesen an den Repeater senden. Dann 10x auf "Send" klicken, um 10 Customer Feedbacks in unter 20 Sekunden zu erzeugen.

![JSBild](Bilder/captcha1.png)
