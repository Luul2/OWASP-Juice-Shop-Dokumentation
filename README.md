# OWASP-Juice-Shop-Dokumentation
Der OWASP Juice Shop wird von der OWASP Foundation für Lernzwecke zur Verfügung gestellt. Dabei handelt es sich um eine absichtlich verwundbare Webanwendung, die entwickelt wurde, um typische Sicherheitslücken (z. B. SQL Injection, Cross-Site Scripting und Broken Access Control) kontrolliert auszunutzen. 
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

Um den Container nach einem Systemneustart zu starten, kann folgender Befehl verwendet werden:

    sudo docker start juice-shop

# Lösungen

## Level 1 Challenges
- [X] [Bonus Payload](../main/Level1/bonus-payload.md) - Use the bonus payload in the DOM XSS Challenge.
- [X] [Mass Dispel](../main/Level1/mass-dispel.md) - Close multiple "Challenge solved"-notifications in one go.
- [X] [Confidential Document](../main/Level1/confidential-document.md) - Access a confidential document.
- [X] [DOM XSS](../main/Level1/dom-xss.md) - Perform a DOM XSS attack with <iframe src="javascript:alert(`xss`)">.
- [X] [Error Handling](../main/Level1/error-handling.md) - Provoke an error that is neither very gracefully nor consistently handled.
- [X] [Exposed Metrics](../main/Level1/exposed-metrics.md) - Find the endpoint that serves usage data to be scraped by a popular monitoring system.
- [X] [Missing Encoding](../main/Level1/missing-encoding.md) - Retrieve the photo of Bjoern's cat in "melee combat-mode".
- [X] [Outdated Allowlist](../main/Level1/outdated-allowlist.md) - Let us redirect you to one of our crypto currency addresses which are not promoted any longer.
- [X] [Privacy Policy](../main/Level1/privacy-policy.md) - Read our privacy policy.
- [X] [Repetitive Registration](../main/Level1/repetitive-registration.md) - Follow the DRY principle while registering a user. 
- [X] [Score Board](../main/Level1/scoreboard.md) - Find the carefully hidden 'Score Board' page.
- [X] [Zero Stars](../main/Level1/zerostars.md) - Give a devastating zero-star feedback to the store.
- [X] [Web3 Sandbox](../main/Level1/web3-sandbox.md) - Find an accidentally deployed code sandbox for writing smart contracts on the fly.

## Level 2 Challenges
- [X] [Admin Section](../main/Level2/admin-section.md) - Access the administration section of the store.
- [X] [Deprecated Interface](../main/Level2/deprecated-interface.md) - Use a deprecated B2B interface that was not properly shut down.
- [X] [Exposed credentials](../main/Level2/exposed-credentials.md) - A developer was careless with hardcoding unused, but still valid credentials for a testing account on the client-side.
- [X] [Empty User Registration](../main/Level2/empty-user-registration.md) - Register a user with an empty email and password.
- [X] [Five-Star Feedback](../main/Level2/5-star-feedback.md) - Get rid of all 5-star customer feedback.
- [X] [Login Admin](../main/Level2/login-admin.md) - Log in with the administrator's user account.
- [X] [Login MC SafeSearch](../main/Level2/login-mc-safesearch.md) - Log in with MC SafeSearch's original user credentials without applying SQL Injection or any other bypass.
- [X] [Meta Geo Stalking](../main/Level2/meta-geo-stalking.md) - Determine the answer to John's security question by looking at an upload of him to the Photo Wall and use it to reset his password via the Forgot Password mechanism.
- [X] [NFT Takeover](../main/Level2/nft-takeover.md) - Take over the wallet containing our official Soul Bound Token (NFT).
- [X] [Password Hash Leak](../main/Level2/password-hash-leak.md) - Obtain the password (hash) of the currently logged-in user directly from a REST API endpoint.
- [X] [Password Strength](../main/Level2/password-strength.md) - Log in with the administrator's user credentials without previously changing them or applying SQL Injection.
- [X] [Security Policy](../main/Level2/security-policy.md) - Behave like any "white-hat" should before getting into the action.
- [X] [View Basket](../main/Level2/view-basket.md) - View another user's shopping basket.
- [X] [Visual Geo Stalking](../main/Level2/visual-geo-stalking.md) -Determine the answer to Emma's security question by looking at an upload of her to the Photo Wall and use it to reset her password via the Forgot Password mechanism.
- [X] [Weird Crypto](../main/Level2/weird-crypto.md) - Inform the shop about an algorithm or library it should definitely not use the way it does.


## Level 3 Challenges
- [] [Admin Registration](../main/Level3/admin-registration.md) - Register as a user with administrator privileges.
- [] [Bjoern’s Favorite Pet](../main/Level3/bjoerns-favorite-pet.md) - Reset the password of Bjoern's OWASP account via the Forgot Password mechanism with the original answer to his security question.
- [] [CAPTCHA Bypass](../main/Level3/CAPTCHA-bypass.md) - Submit 10 or more customer feedbacks within 20 seconds.
- [] [CSRF](../main/Level3/CSRF.md) - Change the name of a user by performing Cross-Site Request Forgery from another origin.
- [] [Database Schema](../main/Level3/database-schema.md) - Exfiltrate the entire DB schema definition via SQL Injection.
- [] [Deluxe Fraud](../main/Level3/deluxe-fraud.md) - Obtain a Deluxe Membership without paying for it.
- [] [Forged Feedback](../main/Level3/forged-feedback.md) - Post some feedback in another user's name.
- [] [Forged Review](../main/Level3/forged-review.md) - Post a product review as another user or edit any user's existing review.
- [] [GDPR Data Erasure](../main/Level3/GDPR-data-erasure.md) - Log in with Chris' erased user account.
- [] [Login Amy](../main/Level3/login-amy.md) - Log in with Amy's original user credentials. (This could take 93.83 billion trillion trillion centuries to brute force, but luckily she did not read the "One Important Final Note")
- [] [Login Bender](../main/Level3/login-bender.md) - Log in with Bender's user account.
- [] [Login Jim](../main/Level3/login-jim.md) - Log in with Jim's user account.
- [] [Manipulate Basket](../main/Level3/manipulate-basket.md) - Put an additional product into another user's shopping basket.
- [] [Mint the Honey Pot](../main/Level3/mint-the-honey-pot.md) - Mint the Honey Pot NFT by gathering BEEs from the bee haven.
- [] [Payback Time](../main/Level3/payback-time.md) - Place an order that makes you rich.
- [] [Privacy Policy Inspection](../main/Level3/privacy-policy-inspection.md) - Prove that you actually read our privacy policy.
- [] [Product Tempering](../main/Level3/product-tempering.md) - Change the href of the link within the OWASP SSL Advanced Forensic Tool (O-Saft) product description into https://owasp.slack.com.
- [] [Reset Jim's Password](../main/Level3/reset-jims-password.md) - Reset Jim's password via the Forgot Password mechanism with the original answer to his security question.
- [] [Upload Size](../main/Level3/upload-size.md) - Upload a file larger than 100 kB.
