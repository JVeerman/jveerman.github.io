---
layout: post
title:  "Passwords!"
date:   2020-02-02 19:38:21 -0500
categories: passwords
---

It is increasingly important to use a password manager.

Choosing a Password Manager

Although this blog post is as of right now, it is important to never be dependant on any tool. As new information comes out about these password managers, such as new critical security vulnerabilities, we need to always be agile enough to drop them and switch to an alternative. Exporting your data from one manager and importing to another is generally very easy.

Factors when choosing a password manager:
security of the solution
privacy stance of the publisher (including whether they are open source)
ease of use with your devices
price

Major Competitors

Recommendation

BitWarden
BitWarden is open source, while LastPass is not.
Security issues found in LastPass recently.
Price differences



Accessing your Password Vault

Masterpassword
Add MFA, supports:
Authenticator apps. You don’t need to choose the Google Authenticator app even if a website appears to only allow that. Other alternatives include Authy, FreeOTP(I use this one)
YubiKey OTP Security Key
Duo
FIDO U2F Security Key
Email (I suggest not using email or SMS)

Physical Tokens
Currently using YubiKey:
One that lives in my laptop(USB-C -> YubiKey 5C Nano)
One that is on my keychain (USB-C -> YubiKey 5C)

Recovery Code
Essential incase all else fails.
Should live in a safe physical location, such as an actual vault.

Features of your Password Manager
1. Autofill
I highly suggest to not use any autofill features used in password managers as there are working proofs of concepts that would exploit this feature to exfiltrate the credentials.
https://www.cs.columbia.edu/~suman/docs/suman_pwdmgr.pdf

2. Auditing Passwords

Exposed Passwords Report






