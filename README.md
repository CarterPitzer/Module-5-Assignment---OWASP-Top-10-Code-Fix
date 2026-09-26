Broken Access Control

Anyone can change the userId in the URL and see another user’s profile.
Fix: Only allow access if the logged‑in user’s ID matches the requested ID.
OWASP: Broken Access Control

Anyone can load any account by changing the ID.
Fix: Only return the account if it belongs to the current user.
OWASP: Broken Access Control

Cryptographic Failures

MD5 is weak and easy to crack.
Fix: Use PBKDF2, bcrypt, or Argon2.
OWASP: Cryptographic Failures

SHA‑1 is weak and unsalted.
Fix: Use bcrypt.
OWASP: Cryptographic Failures

Injection

SQL query uses string concatenation.
Fix: Use prepared statements.
OWASP: Injection

NoSQL query uses raw user input.
Fix: Validate username before querying.
OWASP: Injection

Insecure Design

Password resets happen with only an email.
Fix: Require a secure reset token.
OWASP: Insecure Design

Software and Data Integrity Failures

Loads external script with no integrity check.
Fix: Use Subresource Integrity (SRI).
OWASP: Software and Data Integrity Failures

Server-Side Request Forgery

Fetches any URL the user enters.
Fix: Only allow approved domains.
OWASP: SSRF

Identification and Authentication Failures

Compares plaintext passwords.
Fix: Store and check hashed passwords (bcrypt).
OWASP: Identification and Authentication Failures
