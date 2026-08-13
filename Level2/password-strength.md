## Password Strength

Mit einem Konto aus Juice Shop anmelden und den dabei entstehenden Datenverkehr mit Burp Suite abfangen.

![JSBild](Level2/Bilder/passwordstrength.png)

![JSBild](Level2/Bilder/passwordstrength2.png)

Anschließend wird der abgefangene Login-Request an den Intruder gesendet. Dort wird das Passwort markiert und mit Add als Payload-Position hinzugefügt. Dann als Payload eine Wortliste hinterlegen und den Angriff starten.

![JSBild](Level2/Bilder/passwordstrength3.png)

Bei der Auswertung der Ergebnisse ist zu erkennen, dass der Versuch mit dem Passwort admin123 erfolgreich war. 

![JSBild](Level2/Bilder/passwordstrength4.png)
