## Password Hash Leak 

Mit einem Konto anmelden und währenddessen im Browser-Inspector den Netzwerkverkehr überwachen. 

![JSBild](Level2/Bilder/passwordhashleak1.png)

Dabei fällt auf, dass der Endpunkt whoami?fields=email existiert. 

![JSBild](Level2/Bilder/passwordhashleak2.png)

Anschließend prüfen, ob sich diese Information in Verbindung mit dem Parameter password verwenden lässt.

![JSBild](Level2/Bilder/passwordhashleak3.png)
