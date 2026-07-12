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

Nach einem Neustart kann der Container mit dem folgenden Befehl erneut gestartet werden:

    sudo docker start juice-shop

# Lösungen

## Level 1 Challenges
- [ ] [Bonus Payload](../master/Level1/dom-xss.md) - Use the bonus payload in the DOM XSS Challenge.
- [ ] [Mass Dispel](../master/Level1/bully-chatbot.md) -Close multiple "Challenge solved"-notifications in one go.
- [ ] [Confidential Document](../master/Level1/confidential-doc.md) - Access a confidential document.
- [ ] [DOM XSS](../master/Level1/dom-xss.md) - Perform a DOM XSS attack with <iframe src="javascript:alert(`xss`)">.
- [ ] [Error Handling](../master/Level1/error-handling.md) - Provoke an error that is neither very gracefully nor consistently handled.
- [ ] [Exposed Metrics](Level1/exposed-metrics.md) - Find the endpoint that serves usage data to be scraped by a popular monitoring system.
- [ ] [Missing Encoding](../master/Level1/missing-encoding.md) - Retrieve the photo of Bjoern's cat in "melee combat-mode".
- [ ] [Outdated Allowlist](../master/Level1/outdated-whitelist.md) Let us redirect you to one of our crypto currency addresses which are not promoted any longer.
- [ ] [Privacy Policy](../master/Level1/privacy-policy.md) - Read our privacy policy.
- [ ] [Repetitive Registration](../master/Level1/repeat-register.md) - Follow the DRY principle while registering a user. 
- [ ] [Score Board](../master/Level1/score-board.md) - Find the carefully hidden 'Score Board' page.
- [ ] [Zero Stars](../master/Level1/zero-stars.md) - Give a devastating zero-star feedback to the store.
- [ ] [Web3 Sandbox](../master/Level1/web3-sandbox.md) - Find an accidentally deployed code sandbox for writing smart contracts on the fly.
