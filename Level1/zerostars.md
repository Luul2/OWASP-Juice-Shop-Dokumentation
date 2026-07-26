## Zero-Stars

In Burp Suite über Proxy -> Intercept auf Open Browser gehen. Dann in diesem die Seite aufrufen, auf der das Feedback abgegeben werden kann und die Felder ausfüllen:

![JSBild](Level1/Bilder/zerostars1.png)

Nachdem das Feedback gesendet wurde, wird der zugehörige HTTP-Request in Burp Suite abgefangen. Dieser kann unter Proxy → HTTP history eingesehen und analysiert werden. Anschließend wird der Request an den Repeater gesendet, um die übermittelten Parameter gezielt zu verändern:

![JSBild](Level1/Bilder/zerostars2.png)

Im Repeater wird die abgegebene Bewertung gesucht und der ursprüngliche Wert von 3 auf 0 geändert:

![JSBild](Level1/Bilder/zerostars3.png)

Zum Schluss wird der manipulierte Request erneut an den Server gesendet, wodurch die 0-Sterne-Bewertung erfolgt:

![JSBild](Level1/Bilder/zerostars4.png)
