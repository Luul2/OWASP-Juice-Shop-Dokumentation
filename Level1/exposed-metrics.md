## Exposed Metrics

Um den versteckten Monitoring-Endpunkt zu finden, wurde die Standardkonfiguration von Prometheus überprüft. Prometheus verwendet werksseitig den Pfad /metrics, um Messdaten von Anwendungen abzurufen.

Durch Aufrufen von:

    http://127.0.0.1:3000/metrics

Erscheint eine Seite mit internen Informationen über die Anwendung, darunter Prozessinformationen wie CPU-Auslastung oder Speicherverbrauch:

![JSBild](Level2/Bilder/exposedmetrics.png)
