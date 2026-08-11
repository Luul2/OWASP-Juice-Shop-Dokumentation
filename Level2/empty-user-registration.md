## Empty user registration

Zunächst im Juice Shop zur Benutzerregistrierung navigieren und beliebige Daten eingeben. Anschließend Burp Suite öffnen und Interception aktivieren. Danach auf "Register" klicken. 

![JSBild](Level2/Bilder/emptyuserregistration1.png)

In Burp Suite lässt sich nun der entsprechende Request abfangen und bearbeiten. Dabei werden die Werte für E-Mail-Adresse und Passwort aus dem Request entfernt.

![JSBild](Level2/Bilder/emptyuserregistration2.png)

Zum Schluss den manipulierten Request weiterleiten. 
