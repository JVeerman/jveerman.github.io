---
layout: post
title:  "Managing Your Passwords"
date:   2020-02-02 19:38:21 -0500
categories: passwords
---

A forum you used in 2012 has been compromised and has had all its users' data leaked. 
Among that data was your regular username of JSmith44, your email jsmith44@gmail.com and your password hunter2.
The data was sold to the highest bidder on the darkweb and purchaser(let's call him Mr X) is trying to see whether any of the users' credentials could be used for more important accounts, such as for banking.
Lucky for Mr X(and unlucky for you), the password that you used for the forum is actually the same password for your gmail account. 

What would Mr X be able to do if they had your gmail account? How could this have been prevented? How can you protect yourself now? What if in this scenario it was only your Netflix account sharing a password instead of your gmail account?

## Password Best Practises

If the password for the forum were unique and only used for that forum, then the credentials would not have worked for your gmail. It is difficult to have a unique and complex password for every account you have, but it is very easy to accomplish with a password manager.
A password manager will help you generate a very complex passwords and save them for you to access on any of your devices. 

If the password you used for the forum were actually used for your gmail, having had setup multi-factor authentication on your gmail account would have stopped Mr X from logging in. Multi-factor authentication is when authentication requires two or more pieces of evidence. Typically this is a password but if you add a physical or digital token(like an RSA token or a Google Authenticator code) to your account as required to login, then Mr X would not be able to login with just a password.

  * Use complex and unique passwords
  * Use a trusted and secure password manager
  * Use multi-factor authentication

## Benefits of a Password Manager

1. Security. 
  * Your passwords are stored encrypted in a way that only you have access to them.
1. Less to Memorize and Never Forget. 
  * You only need to remember one master password for your password manager. You will also never have to use Forgot Password again!
2. Use Complex and Unique Passwords.
  * Allows you to adhere to password best practises. It is virtually impossible to have a unique 14 digit alphanumeric string for every account you have without a password manager.
2. Easy Password Creation.
  * Ability to quickly generate new secure passwords with the click of a button. 
3. Seamlessly Login. 
  * Logging in can actually be less clicks with a password manager.
4. Auditing Capabilities. 
  * You can run reports to see the strength of your passwords and whether any of them are at risk of being compromised.


## Choosing a Password Manager

It is important to never be overly dependant on any tool to the point that it is irreplaceable. As new information comes out about these password managers, such as new critical security vulnerabilities, we need to always be agile enough to drop them and switch to an alternative. Exporting your data from one manager and importing to another is generally very easy.

For my purposes, I wanted a password manager that met the following:
1. Cloud-based
2. Securely stores my passwords
2. Mobile and Desktop support
2. Browser extension for my browsers(Brave and FireFox)
2. Allows for use of physical tokens for multi-factor authentication
3. Open source preferred
4. Reasonably priced

### Major Competitors

| Name     | Security Vulnerability History | Mobile and Desktop Support? | Browser extension support? | Open Source? | Price |
| LastPass | 2 High, 1 Medium        [Details](https://nvd.nist.gov/vuln/search/results?form_type=Basic&results_type=overview&query=lastpass&search_type=all)       | Yes                         | Yes                        | No           | LastPass has a free plan, which is good. For $3/month, you get 1GB encrypted file storage, secured sharing, Yubikey and Sesame 2FA support, and an ad-free vault.   |
| BitWarden | 1 High              [Details](https://nvd.nist.gov/vuln/search/results?form_type=Basic&results_type=overview&query=bitwarden&search_type=all)          | Yes                         | Yes                        | Yes          | Bitwarden also has a free plan but with one additional feature. The ability to self-host it on your server. For $10 per year, you get 1GB encrypted file storage, sharing for two users, 2FA support for Yubikey, and advanced reports.   |

### Recommendation

I have used both LastPass and Bitwarden extensively over several months and I have chosen BitWarden. I prefer every aspect of BitWarden over LastPass and the fact that BitWarden is open source gives me some assurance that it isn't doing anything unexpected such as sending my credentials to a 3rd party.

## Accessing your Password Vault

### Masterpassword
Add MFA, supports:
* Authenticator apps. You don’t need to choose the Google Authenticator app even if a website appears to only allow that. Other alternatives include Authy, FreeOTP(I use this one)
* YubiKey OTP Security Key
* Duo
* FIDO U2F Security Key
* Email (I suggest not using email or SMS)

### Physical Tokens
Currently using YubiKey:
* One that lives in my laptop(USB-C -> YubiKey 5C Nano)
* One that is on my keychain (USB-C -> YubiKey 5C)

### Recovery Code
Essential incase all else fails.
Should live in a safe physical location, such as an actual vault.

### Autofill Feature - Not Recommended

I highly suggest to not use any autofill features used in password managers as there are working proofs of concepts that would exploit this feature to exfiltrate the credentials.
[Password Managers: Attacks and Defenses](https://www.cs.columbia.edu/~suman/docs/suman_pwdmgr.pdf)


## Audit your Passwords

Most password managers have the feature to audit your passwords for best practises, such as whether the password is complex enough or if the website was compromised.

### Detection of Insecure Passwords

Run the following reports on your password manager and fix any issues found.

1. Reused Passwords Report
* If a service that you use is compromised, reusing the same password elsewhere can allow hackers to easily gain access to more of your online accounts. You should use a unique password for every account or service.

2. Weak Passwords Report
* Weak passwords can easily be guessed by hackers and automated tools that are used to crack passwords. The Bitwarden password generator can help you create strong passwords.

3. Unsecured Websites Report
* Using unsecured websites with the http:// scheme can be dangerous. If the website allows, you should always access it using the https:// scheme so that your connection is encrypted.

4. Inactive 2FA Report
* Two-factor authentication (2FA) is an important security setting that helps secure your accounts. If the website offers it, you should always enable two-factor authentication.


### Detection of Compromised Accounts 


1. Exposed Passwords Report
* Exposed passwords are passwords that have been uncovered in known data breaches that were released publicly or sold on the dark web by hackers.

2. Data Breach Report
* A "breach" is an incident where a site's data has been illegally accessed by hackers and then released publicly. Review the types of data that were compromised (email addresses, passwords, credit cards etc.) and take appropriate action, such as changing passwords.

3. Financial Statements
* Although not part of the password manager, I suggest checking your financial statements regularly(or better yet, enable notifications for every purchase). The credit card companies do their best to detect fraud, however if the fraudulent purchase might fit the characteristics of a legitimate purchase and not be considered a fraudulent purchase at first. This might happen, for instance, if your inactive Netflix account were compromised and the malicious person reactivated the account for the premium service.
* By validating all your purchases, any instances of a compromised account with your saved payment details will be caught early and prevent any losses. 

### Final Words

It is becoming increasingly difficult to ensure that all our passwords are secure. A password manager will help make sure that Mr X will not be able to compromise your accounts.




