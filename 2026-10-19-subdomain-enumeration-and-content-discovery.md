Daily Cybersecurity Learning Log

Date: 19 October 2026
Focus: Subdomain Enumeration and Web Content Discovery

1. Subdomain Enumeration

Learned about subdomain enumeration as part of reconnaissance and information gathering in web security.

- Passive enumeration: Collecting information from existing sources without directly probing the target's infrastructure.
- Active enumeration: Sending queries or probes to identify subdomains, which may interact directly with the target's infrastructure.
- Tool used: Subfinder
- Objective: Discover subdomains associated with a domain to help understand its potential attack surface.

2. Web Content and Directory Discovery

Practised web content discovery using:

- ffuf: Used with a wordlist to identify potentially accessible paths and resources.
- Feroxbuster: Used with SecLists wordlists for directory and content discovery.
- Practice target: "testphp.vulnweb.com"

Key Takeaways

- Subdomain enumeration helps identify additional hosts associated with a domain.
- Passive and active enumeration differ in how they collect information and interact with the target.
- Wordlist-based content discovery helps identify potentially interesting web paths that may not be linked from the main page.
- Discovered paths and subdomains require further verification; discovery alone does not establish a vulnerability.

Practical Evidence

Attach terminal screenshots showing the actual commands used and relevant results. Redact any sensitive information and distinguish confirmed findings from potential discoveries.

Scope note: Use these techniques only on systems you own or have explicit permission to test, including designated training environments.
