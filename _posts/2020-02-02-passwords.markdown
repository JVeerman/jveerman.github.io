---
layout: post
title:  "Passwords Management for 2020"
date:   2020-02-02 19:38:21 -0500
categories: passwords
---

## Password Managers are Essential

It is increasingly important to use a password manager.

## Choosing a Password Manager

Although this blog post is as of right now, it is important to never be dependant on any tool. As new information comes out about these password managers, such as new critical security vulnerabilities, we need to always be agile enough to drop them and switch to an alternative. Exporting your data from one manager and importing to another is generally very easy.

For my purposes, I wanted a password manager that met the following:
1. Cloud-based
2. Securely stores my passwords
2. Mobile and Desktop support
2. Browser extension for my browsers(Brave and FireFox)
3. Open source preferred
4. Reasonably priced

# Major Competitors

| Name     | Security Vulnerability History | Mobile and Desktop Support? | Browser extension support? | Open Source? | Price |
| LastPass | 2 High, 1 Medium        [Details](https://nvd.nist.gov/vuln/search/results?form_type=Basic&results_type=overview&query=lastpass&search_type=all)       | Yes                         | Yes                        | No           | LastPass has a free plan, which is good. For $3/month, you get 1GB encrypted file storage, secured sharing, Yubikey and Sesame 2FA support, and an ad-free vault.   |
| BitWarden | 1 High              [Details](https://nvd.nist.gov/vuln/search/results?form_type=Basic&results_type=overview&query=bitwarden&search_type=all)          | Yes                         | Yes                        | Yes          | Bitwarden also has a free plan but with one additional feature. The ability to self-host it on your server. For $10 per year, you get 1GB encrypted file storage, sharing for two users, 2FA support for Yubikey, and advanced reports.   |

# Security Vulnerability History

As mentioned above, there were vulnerabilities found in all the tools.






# Recommendation

BitWarden





## Accessing your Password Vault

# Masterpassword
Add MFA, supports:
Authenticator apps. You don’t need to choose the Google Authenticator app even if a website appears to only allow that. Other alternatives include Authy, FreeOTP(I use this one)
YubiKey OTP Security Key
Duo
FIDO U2F Security Key
Email (I suggest not using email or SMS)

# Physical Tokens
Currently using YubiKey:
One that lives in my laptop(USB-C -> YubiKey 5C Nano)
One that is on my keychain (USB-C -> YubiKey 5C)

# Recovery Code
Essential incase all else fails.
Should live in a safe physical location, such as an actual vault.

# Features of your Password Manager
1. Autofill
I highly suggest to not use any autofill features used in password managers as there are working proofs of concepts that would exploit this feature to exfiltrate the credentials.
[Password Managers: Attacks and Defenses](https://www.cs.columbia.edu/~suman/docs/suman_pwdmgr.pdf)

2. Auditing Passwords

Exposed Passwords Report






