## Weird Crypto

Der Quellcode des Juice Shops ist öffentlich einsehbar. Bei einer genaueren Betrachtung fällt auf, dass MD5 als Hash-Algorithmus verwendet wird.

![JSBild](Level2/Bilder/weirdcrypto.png)

Anschließend habe ich überprüft, ob diese Funktion auch für Passwörter verwendet wird. In models/user.js findet sich dazu der folgende Code:

![JSBild](Level2/Bilder/weirdcrypto1.png)

Hier wird das Klartextpasswort an security.hash() übergeben und somit mit MD5 gehasht, bevor es als Passwortwert gespeichert wird.

Um den Juice Shop darüber zu informieren, wird ein Feedback erstellt mit md5 als Information

![JSBild](Level2/Bilder/weirdcrypto2.png)
