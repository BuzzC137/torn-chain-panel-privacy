Privacy Policy

Last updated: August 2025


---

1. Overview

Torn Chain Panel helps authorized Torn players fetch and manage chain numbers with alerts and faction queue control. This policy explains what user data is collected, how it is used, and how you can control it.


---

2. Data Collected & Usage

Verified Torn username: Stored locally to namespace settings and fetch chain numbers.

Authentication credentials: Admin PIN and authorization token used to protect sensitive functionality. These are stored in localStorage / sessionStorage.

Torn API key: Provided by the user to import faction members via YATA. Used only in-session to query yata.yt; not exfiltrated elsewhere.

UI preferences & state: Volume, alert thresholds, flashing settings, panel position, and queue contents. Stored locally to persist user configuration.

Page context: The extension injects UI into the Torn page. It does not harvest browsing history beyond operating on that page.



---

3. Sharing & Third Parties

No user data is sold. External requests (e.g., to YATA or the chain resolution backend) occur only when explicitly initiated by the user (e.g., entering their Torn API key or clicking "Get My #"). Credentials are kept local unless included in those explicit requests.


---

4. Security

Sensitive data is stored in the browser's localStorage or sessionStorage. Admin access is protected by a 4-digit PIN that unlocks per session. Authorization tokens can be validated server-side if configured. All external communication uses HTTPS.


---

5. User Control & Revocation

Users can clear stored data via browser developer tools by removing entries from localStorage or sessionStorage. Authorization can be revoked by invalidating tokens if server-side validation is used.


---

6. Data Minimization

The extension collects only what is necessary for its single purpose: managing chain numbers and related alerts/queue state. It does not collect health, financial, location (beyond normal Torn.com access), or personal communication data.


---

7. Contact

For support or reporting issues: Discord BuzzC137


---

By using Torn Chain Panel you acknowledge and agree to this privacy policy.
