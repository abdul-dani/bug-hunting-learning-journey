File Path Traversal and OS Command Injection

Date: November 2, 2026
Platform: PortSwigger Web Security Academy
Category: Web Application Security

1. File Path Traversal – Bypassing a Blocked Traversal Sequence

What I learned

File path traversal is a vulnerability that occurs when an application allows users to access files outside the intended directory because user-supplied file paths are not properly validated.

Lab practice

- Practised a lab where traversal sequences were blocked.
- Learned that an absolute path could be used to bypass the traversal sequence restriction.
- Understood why simply blocking traversal patterns is not sufficient protection.

Security lesson

Applications should validate file paths against an approved base directory and prevent access to files outside that directory.

2. OS Command Injection – Simple Case

What I learned

OS command injection occurs when an application passes unsanitized user input to an operating system command, potentially allowing an attacker to execute unintended commands.

Lab practice

- Studied a simple OS command injection vulnerability.
- Learned how unsafe handling of user input can expose operating system command execution.
- Understood the importance of secure input handling.

Security lesson

Developers should avoid constructing operating system commands directly from user input. Where command execution is necessary, use safe APIs, strict input validation, and least-privilege permissions.

Key Takeaways

1. Blocking known traversal sequences alone does not prevent file path traversal.
2. Absolute paths can sometimes bypass weak path restrictions.
3. Unsanitized user input passed to operating system commands can lead to OS command injection.
4. Proper input validation and secure application design are essential.

Practice environment: PortSwigger Web Security Academy
Scope: Authorized security training labs.
