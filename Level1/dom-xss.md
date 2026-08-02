## DOM-XSS

Mit der nachfolgenden Payload kann überprüft werden, ob eingeschleuster JavaScript-Code vom Browser ausgeführt wird:

    <iframe src="javascript:alert('xss')">

Die Funktion alert() erzeugt dabei ein Dialogfenster, bei dem der eingegebene Wert 'xss' als Inhalt der Meldung angezeigt wird und beliebig verändert werden kann.

![JSBild](Level1/Bilder/xss1.png)

![JSBild](Level1/Bilder/xss2.png)

Die Anwendung ist somit anfällig für XSS, da der eingeschleuste JavaScript-Code vom Browser ausgeführt und nicht als reiner Text behandelt wird. 
