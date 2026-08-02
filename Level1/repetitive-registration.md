## Repetitive Registration

Die HTTP-Anfrage zur Registrierung eines neuen Benutzers mit Burp Suite abfangen. Dazu in Juice Shop einen neuen Benutzer registrieren:

![JSBild](Level1/Bilder/repetitivereg1.png)   

Anschließend in Burp Suite nach der Abfrage suchen und den Wert aus dem Feld password oder passwordRepeat verändern, damit die beiden Werte nicht mehr übereinstimmen. Jetzt kann die manipulierte Anfrage an den Server weitergeleitet werden.

![JSBild](Level1/Bilder/repetitivereg2.png)  

Da die Anwendung die Übereinstimmung der beiden Passwortfelder nicht serverseitig überprüft, wird die Registrierung trotz unterschiedlicher Passwörter akzeptiert.
