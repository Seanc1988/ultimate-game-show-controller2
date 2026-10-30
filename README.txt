THE FEUD LIVE 2.4.1 — PHONE PAGES

Extract this ZIP. Upload all FOUR HTML files and this README directly into your Feud GitHub repository root. Do not upload the ZIP itself. These HTML files are self-contained: separate css/js/assets folders are not needed on the phone website.

index.html — landing page
host-controller.html — private host remote
signup.html — audience contestant signup
buzzer.html — Premium team buzzer

Keep your real Wheel repository separate: Seanc1988/ultimate-game-show-controller contains the working Wheel code. The supplied repository with a trailing 2 currently contains partial Feud files, not Wheel code. No repository was modified by this release.

After GitHub Pages is published, set the computer's Contestants → Hosted phone controller URL to the full HTTPS address ending in /buzzer.html. The private host controller automatically uses host-controller.html beside it. Scan the computer's PRIVATE Host phone controller QR to authorize the host phone. Never show that QR to contestants.

Keep the computer/server and audience window running. Internet and PeerJS/WebRTC are required. The phone pages do not run a separate game engine.
