# Email-code verification instead of ITB SSO

Registered users must prove they hold an itb.ac.id email to earn the trust advantage.

Research found ITB's SSO is CAS-based (`login.itb.ac.id/cas/login`) and documented as internal-only ("aplikasi pendukung kegiatan ITB"), with no public OAuth 2.0 / OIDC / LDAP developer access. Integrating SSO would require ITB IT to register us as a client. We decided: user enters an itb.ac.id address and a 6-digit code is emailed to it; mailbox possession is the proof of an ITB account. SSO can replace it later if ITB exposes a client.
