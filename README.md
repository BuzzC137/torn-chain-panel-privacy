Privacy Policy

Last updated: August 2025

Overview

Torn Chain Panel is a tool for authorized Torn players to fetch and manage chain numbers with alerts and faction queue control. This policy explains what data the extension processes, when it is sent off your device, and your choices.

Data We Process
Stored locally in your browser

Verified Torn username – used to namespace settings and fetch your chain number.

Admin PIN and session unlock state – protects admin features (PIN in localStorage; unlock state in sessionStorage).

Authorization token (if you use one) – saved in localStorage to access protected backend routes.

Optional Torn API key (for YATA import) – you enter it; used only during your session to query yata.yt.

UI preferences & state – e.g., volume, alert thresholds, flashing settings, panel position, and queue entries you add.

Local storage means this data stays on your device and is not uploaded by the extension unless you take an action that requires a network request (examples below).

Sent over the network (only when you trigger an action)

Queue / chain requests to our backend at https://tornpanel.online (and subdomains on *.tornpanel.online):

What is sent: your username and the specific action (e.g., enqueue, leave, status).

Purpose: to atomically manage chain positions and return your current status.

Retention: operational logs may contain your username and request metadata. We keep logs only as long as needed for reliability and abuse prevention; current target is ≤30 days. We do not sell, rent, or use this data for advertising or profiling.

Optional YATA import from https://yata.yt/api/v1/faction/members/:

What is sent: the API key you provide, in the request you initiate.

Purpose: to fetch faction members for convenience inside the UI.

Retention: the key is not transmitted to our server; it is used client-side to call YATA. We do not store or share it.

We do not collect browsing history, Google account information, or unrelated page content. The content script only runs on Torn and TornPanel domains as declared in the extension manifest.

Sharing & Sale

We do not sell user data.

We do not share user data with third parties except as required to fulfill your explicit requests (e.g., your YATA call to yata.yt or your chain action to tornpanel.online).

We do not use advertising or analytics trackers.

Security

All network requests use HTTPS.

Sensitive local data (PIN, tokens) live in localStorage/sessionStorage on your device.

Admin unlock is session-scoped.

Server endpoints restrict commands to specific actions and domains.

Permissions (and why)

storage – save your local preferences (volume, alerts, PIN, token, queue list).

alarms – run timer/alert logic reliably in the background.

tabs – send queue updates from the service worker to open Torn/TornPanel tabs.

Host permissions:

https://www.torn.com/* – inject UI only on Torn, to render the panel.

https://tornpanel.online/*, https://*.tornpanel.online/*, https://ui.tornpanel.online/* – talk to the chain backend and bridge script.

(Optional by you) Calls to https://yata.yt/* happen only when you press “Load Members” with your API key.

We do not request activeTab or scripting permissions.

Your Choices & Data Deletion

Clear local data: remove entries via browser developer tools (Application → Local Storage / Session Storage) or uninstall the extension.

Revoke server access: remove/rotate your authorization token; stop using “Get My #” and queue actions.

YATA key: remove it from the UI/session to stop YATA requests.

Server logs: contact us to request deletion; see “Contact” below.

Data Minimization

We collect and transmit only what’s necessary to provide chain queue functionality and optional YATA import. We do not process sensitive categories (health, precise location, financial, etc.).

Children’s Privacy

This extension is intended for general audiences of Torn players and is not directed to children.

Changes to this Policy

If we materially change this policy, we’ll update the “Last updated” date and publish the new version at the same URL.

Contact

Questions or deletion requests: buzzc137+privacy@proton.me (example; replace with your real inbox).
Support: Discord BuzzC137.
