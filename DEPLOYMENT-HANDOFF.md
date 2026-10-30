# Feud phone deployment — 2026-10-30

Published complete self-contained host-controller.html, signup.html, buzzer.html and index.html to Seanc1988/ultimate-game-show-controller2. Baseline: Feud 2.4.0 protocol with existing Wheel-style 2.4.1 phone pages. Fixed missing CSS/JS deployment by embedding dependencies; signup logo resized for mobile delivery. Wheel repository untouched.

## Enable public hosting
In repository Settings > Pages, choose Deploy from a branch, main, /(root), Save. This GitHub connector cannot administer Pages. Public URL returned 404 before publication; hosting activation and final public URL verification remain outstanding.

Expected base URL: https://seanc1988.github.io/ultimate-game-show-controller2/
Set the computer game's Hosted phone controller URL to that base plus buzzer.html. Use computer-generated contestant QR for signup and PRIVATE host QR for host authorization. Opening host-controller.html without pairing is intentionally insufficient.

## Network
GitHub serves static pages; PeerJS/WebRTC connects them to the running PC. PC needs internet. Phones can attempt connection over independent mobile data. Existing baseline STUN/TURN configuration is preserved. Relay credentials/service validity, real carrier NAT, iPhone/Android and venue connectivity have not been verified; GitHub hosting does not guarantee those connections.

## Validation
Ran original host-phone-browser.cjs against the exact bundled pages in a separate phone-sized browser. All assertions passed: pairing, manual buzz, both face-off answers, award/play/pass, TV reveal, duplicate protection, red strikes, undo, steal, next round, responsive dock, disconnect/reconnect without replay, Quick Cash A/B/typing/typos/duplicate/timers/reveal/completion, stale phase rejection, unauthorized denial, revocation, no JS errors. Transport is mocked; this is not a cellular test.

Source assets prepared from /workspace/scratch/707319060ec4/deliverables/phone-controller-v2.4.1. Published pages live at repo root; no game engine or AI credentials added. Keep the host PC and audience window open.
