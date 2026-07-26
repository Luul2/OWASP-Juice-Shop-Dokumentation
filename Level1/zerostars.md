## Zero-Stars

In Burp Suite über Proxy -> Intercept auf Open Browser gehen. Dann in diesem die Seite aufrufen, auf der das Feedback abgegeben werden kann und die Felder ausfüllen:


Nachdem das Feedback gesendet wurde, wird der zugehörige HTTP-Request in Burp Suite abgefangen. Dieser kann unter Proxy → HTTP history eingesehen und analysiert werden. Anschließend wird der Request an den Repeater gesendet, um die übermittelten Parameter gezielt zu verändern:


Im Repeater wird die abgegebene Bewertung gesucht und der ursprüngliche Wert von 3 auf 0 geändert. Zum Schluss wird der manipulierte Request erneut an den Server gesendet. 

