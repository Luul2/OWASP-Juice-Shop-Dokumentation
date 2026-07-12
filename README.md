# OWASP-Juice-Shop-Dokumentation
Der OWASP Juice Shop ist eine absichtlich verwundbare Webanwendung, die entwickelt wurde, um typische Sicherheitslücken moderner Webanwendungen praktisch zu lernen und zu testen.
Diese Dokumentation enthält die Installation mit Docker sowie Lösungen und Walkthroughs zu verschiedenen Aufgaben und Schwachstellen.

**Voraussetzungen:**
- Kali Linux oder anderes Linux-System
- Docker installiert

# Installation von Juice Shop mit Docker

Juice Shop herunterladen:
    
    sudo docker pull bkimminich/juice-shop

Container mit Juice Shop starten:
    
    sudo docker run -d --name juice-shop -p 3000:3000 bkimminich/juice-shop

Prüfung, ob Juice Shop läuft:

    sudo docker ps 

Jetzt kann der Juice shop mit http://localhost:3000 geöffnet werden

Nach einem Neustart kann der Container mit dem folegenden Befehl erneut gestartet werden:

    sudo docker start juice-shop
