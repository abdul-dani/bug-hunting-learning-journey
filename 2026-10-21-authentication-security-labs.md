Authentication Security — Bug Hunting Learning Log

Date: 21 October 2026
Platform: PortSwigger Web Security Academy
Focus: Username Enumeration, Rate-Limit Bypass, and 2FA Authentication

1. Username Enumeration via Response Timing

Learned how differences in server response times can reveal whether a username is valid.

Key takeaway: Even when an application displays similar error messages, timing differences may expose information about account validity.

2. Bypassing IP-Based Rate Limiting

Learned how the "X-Forwarded-For" HTTP header can be used to bypass IP-based rate limiting when an application improperly trusts client-supplied IP information.

Key takeaway: Applications should not blindly trust forwarded-IP headers. These headers must be configured and validated according to a trusted proxy setup.

3. 2FA Simple Bypass

Studied a weakness in multi-factor authentication where flaws in the authentication flow can allow access without properly completing the second-factor verification step.

Key takeaway: The server must enforce second-factor verification before granting access to protected resources.

Practical Work

- Studied username enumeration through response timing.
- Practised testing IP-based rate-limit protections with the "X-Forwarded-For" header.
- Investigated a simple two-factor authentication bypass.
- Completed two assigned labs on PortSwigger Web Security Academy.

Security Lessons

- Avoid leaking account information through response timing or error behaviour.
- Implement rate limiting using trusted client-IP information.
- Enforce multi-factor authentication server-side throughout the authentication flow.
- Test only within authorised environments and document findings responsibly.

Evidence

Attach genuine screenshots of the completed PortSwigger labs and relevant Burp Suite Community Edition results, after removing sensitive information.

Summary

This session strengthened my practical understanding of authentication weaknesses, username enumeration, rate-limiting controls, and multi-factor authentication security as part of my bug hunting journey.
