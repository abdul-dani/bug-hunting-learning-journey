Authentication Security — Bug Hunting Learning Log

Date: 22 October 2026
Platform: PortSwigger Web Security Academy
Focus: Broken 2FA Logic and Stay-Logged-In Cookie Security

1. 2FA Broken Logic

Learned how weaknesses in authentication workflows can allow an attacker to bypass proper two-factor authentication enforcement.

In the lab, the attack involved using the attacker's own credentials alongside a victim's username to exploit the authentication flow without requiring the victim to log in.

Key takeaway: Applications must verify the identity and authentication state of the same user throughout the entire login process.

2. Brute-Forcing a Stay-Logged-In Cookie

Studied how persistent-login cookies can expose weaknesses when their structure and password-hash protection are insufficiently secure.

The lab covered:

- Analysing the cookie structure.
- Understanding how the cookie's contents could be recovered or reproduced.
- Substituting a victim's username in the cookie.
- Brute-forcing weak password-hash protection.

Key takeaway: Persistent-login cookies must be generated securely, protected against tampering, and designed to prevent guessing or forgery.

Practical Achievements

- Completed the 2FA broken logic lab.
- Completed the brute-forcing a stay-logged-in cookie lab.
- Improved my understanding of authentication workflow weaknesses and persistent-session security.

Defensive Lessons

- Enforce 2FA server-side before granting access to protected resources.
- Bind authentication state to the correct user.
- Use secure, unpredictable persistent-session tokens.
- Protect cookie integrity and avoid exposing password-derived values in cookies.
- Apply appropriate expiration, revocation, and session-management controls.

Evidence

Attach genuine screenshots showing both labs marked as solved. Remove session tokens, cookies, credentials, and other sensitive information before sharing.

Summary

This session strengthened my practical understanding of authentication vulnerabilities, two-factor authentication enforcement, and persistent-login cookie security as part of my bug hunting journey.
