# Authentication

Core HTTP/session behavior is implemented under `odoo/http/`. Optional authentication extensions include LDAP, OAuth, signup, passkey, TOTP, password policy, timeout, and portal modules. Registration, reset, MFA enrollment, session lifetime, and provider settings must be verified against the relevant installed addons and configuration; dependency presence alone is not evidence that a control is enabled.
