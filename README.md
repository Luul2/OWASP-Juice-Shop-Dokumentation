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
- [ ] [Bonus Payload](../main/Level1/dom-xss.md) - Use the bonus payload in the DOM XSS Challenge.
- [ ] [Mass Dispel](../main/Level1/bully-chatbot.md) -Close multiple "Challenge solved"-notifications in one go.
- [ ] [Confidential Document](../main/Level1/confidential-doc.md) - Access a confidential document.
- [ ] [DOM XSS](../main/Level1/dom-xss.md) - Perform a DOM XSS attack with <iframe src="javascript:alert(`xss`)">.
- [ ] [Error Handling](../main/Level1/error-handling.md) - Provoke an error that is neither very gracefully nor consistently handled.
- [ ] [Exposed Metrics](../main/Level1/exposed-metrics.md) - Find the endpoint that serves usage data to be scraped by a popular monitoring system.
- [ ] [Missing Encoding](../main/Level1/missing-encoding.md) - Retrieve the photo of Bjoern's cat in "melee combat-mode".
- [ ] [Outdated Allowlist](../main/Level1/outdated-whitelist.md) Let us redirect you to one of our crypto currency addresses which are not promoted any longer.
- [ ] [Privacy Policy](../main/Level1/privacy-policy.md) - Read our privacy policy.
- [ ] [Repetitive Registration](../main/Level1/repeat-register.md) - Follow the DRY principle while registering a user. 
- [X] [Score Board](../main/Level1/scoreboard.md) - Find the carefully hidden 'Score Board' page.
- [ ] [Zero Stars](../main/Level1/zerostars.md) - Give a devastating zero-star feedback to the store.
- [ ] [Web3 Sandbox](../main/Level1/web3-sandbox.md) - Find an accidentally deployed code sandbox for writing smart contracts on the fly.

## Level 2 Challenges
- [ ] [Admin Section](../main/Level2/admin-section.md) - Access the administration section of the store.
- [ ] [Deprecated Interface](../main/Level2/deprecated-interface.md) - Use a deprecated B2B interface that was not properly shut down.
- [ ] [Exposed credentials](../main/Level2/exposed-credentials.md) - A developer was careless with hardcoding unused, but still valid credentials for a testing account on the client-side.
- [ ] [Empty User Registration](../main/Level2/empty-user-registration.md) - Register a user with an empty email and password.
- [ ] [Five-Star Feedback](../main/Level2/5-star-feedback.md) - Get rid of all 5-star customer feedback.
- [ ] [Login Admin](../main/Level2/login-admin.md) - Log in with the administrator's user account.
- [ ] [Login MC SafeSearch](../main/Level2/login-mc-safesearch.md) - Log in with MC SafeSearch's original user credentials without applying SQL Injection or any other bypass.
- [ ] [Meta Geo Stalking](../main/Level2/meta-geo-stalking.md) - Determine the answer to John's security question by looking at an upload of him to the Photo Wall and use it to reset his password via the Forgot Password mechanism.
- [ ] [NFT Takeover](../main/Level2/nft-takeover.md) - Take over the wallet containing our official Soul Bound Token (NFT).
- [ ] [Password Hash Leak](../main/Level2/password-hash-leak.md) - Obtain the password (hash) of the currently logged-in user directly from a REST API endpoint.
- [ ] [Password Strength](../main/Level2/password-strength.md) - Log in with the administrator's user credentials without previously changing them or applying SQL Injection.
- [ ] [Security Policy](../main/Level2/security-policy.md) - Behave like any "white-hat" should before getting into the action.
- [ ] [View Basket](../main/Level2/view-basket.md) - View another user's shopping basket.
- [ ] [Visual Geo Stalking](../main/Level2/visual-geo-stalking.md) -Determine the answer to Emma's security question by looking at an upload of her to the Photo Wall and use it to reset her password via the Forgot Password mechanism.
- [ ] [Weird Crypto](../main/Level2/weird-crypto.md) - Inform the shop about an algorithm or library it should definitely not use the way it does.
