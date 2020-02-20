---
layout: post
title:  "Managing Your Passwords"
date:   2020-02-16 19:54:21 -0500
categories: passwords
---

A forum you used in 2012 has been compromised and has had all its users' data leaked. 
Among that data was your regular username of JSmith44, your email jsmith44@gmail.com and your password hunter2.
The data was sold to the highest bidder on the darkweb and purchaser(let's call him Mr X) is trying to see whether any of the users' credentials could be used for more important accounts, such as for banking.
Lucky for Mr X(and unlucky for you), the password that you used for the forum is actually the same password for your gmail account. 

What would Mr X be able to do if they had your gmail account? How could this have been prevented? How can you protect yourself now?

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

In my opinion password managers in this day and age must be able to achieve the following:
1. Securely store passwords
* Confidentiality: Only you should be able to see your saved passwords. Your password manager should use robust end-to-end encryption such that noone, not even the password manager service, should be able to read your password.
* Authentication/Authorization: Secure access
2. Cloud based 
3. Mobile and Desktop support
3. Browser extension support
4. Actively developed
* Certain browsers such as Google Chrome and FireFox have built-in password management capabilities, however they are not robust in features or actively developed as there are many competing priorities.
5. Independently audited



For my purposes, I also wanted some additional features:

2. Allows for use of physical tokens for multi-factor authentication
3. Open source preferred
4. Reasonably priced
4. Dark  mode
* It is very minor, but I had to note it! 

### Major Competitors

| Password Manager     | Features List                                                      | Cloud Based | Actively Developed | Independently Audited   |  Mobile and Desktop Support        | Browser Integration      | Open Source  | Free Plan Option | Physical Token MFA | Dark-Mode | Linux Support | Monthly Price (USD) | Google Play # of Downloads | Google Play Rating |                                                                                                                                                                                                                                      |
| LastPass             | https://www.lastpass.com/enterprise/enterprise-features            | Yes         | Yes                | No                      | Yes                                | Yes                      | No           | Yes              | Yes                | No        | Yes           | $3                  | 5M+                        | 4.3 / 5            | 
| BitWarden            | https://bitwarden.com/                                             | Yes         | Yes                | No                      | Yes                                | Yes                      | Yes          | Yes              | Yes                | Yes       | Yes           | $0.83               | 500K+                      | 4.6 / 5            | 
| 1Password            | https://1password.com/sign-up/                                     | Yes         | Yes                | No                      | Yes                                | Yes                      | No           | Yes              | Yes                | No        | Yes           | $3                  | 1M+                        | 4.2 / 5            | 
| Dashlane             | https://www.dashlane.com/business/features                         | Yes         | Yes                | No                      | Yes                                | Yes                      | No           | Yes              | Yes                | Yes       | Yes           | $3.33               | 1M+                        | 4.6 / 5            | 
| KeePass              | https://keepass.info/features.html                                 | No          | Yes                | No                      | Yes, through 3rd parties           | Yes, through 3rd parties | Yes          | Yes              | Yes                | No        | Yes           | Free                | 1M+                        | 4.6 / 5            | 
| Keeper               | https://www.keepersecurity.com/personal.html                       | Yes         | Yes                | No                      | Yes                                | Yes                      | No           | No               | Yes                | Yes       | Yes           | $2.49               | 10M+                       | 4.6 / 5            | 

### Security Vulnerability History

The following is the history of reported vulnerabilities in the cloud-based password managers. 

| Password Manager     | Vulnerabilities Reported           |  Details                                                   |
| LastPass             | 2 High, 2 Medium                   | [Details](https://nvd.nist.gov/vuln/search/results?form_type=Basic&results_type=overview&query=lastpass&search_type=all) |
| BitWarden            |                                    | [Details](https://nvd.nist.gov/vuln/search/results?form_type=Basic&results_type=overview&query=bitwarden&search_type=all) |
| 1Password            | 4 Medium                           | [Details](https://nvd.nist.gov/vuln/search/results?form_type=Advanced&results_type=overview&query=1password&search_type=all) |
| Dashlane             | 1 High                             | [Details](https://nvd.nist.gov/vuln/search/results?form_type=Advanced&results_type=overview&query=dashlane&search_type=all) |
| KeePass              | 1 Critical(*), 4 High, 2 Medium    | [Details](https://nvd.nist.gov/vuln/search/results?form_type=Advanced&results_type=overview&query=keepass&search_type=all) |
| Keeper               | N/A                                |                         |                                                    

Note(*): Part of an unofficial contribution for using on Android

### Password Manager Recommendation

I have used both LastPass and Bitwarden extensively over several months and I have chosen BitWarden. I prefer every aspect of BitWarden over LastPass and the fact that BitWarden is open source gives me some assurance that it isn't doing anything unexpected such as sending my credentials to a 3rd party.

## Accessing your Password Manager

### Enabling Multi-Factor Authentication

Password managers are typically accessed with a username and password. For added assurance that only you can access your password manager, I suggest enabling multi-factor authentication for atleast two other factors. For example, I use a physical token and an authenticator app.

Most password managers support:
* Authenticator apps. You don’t need to choose the Google Authenticator app even if a website appears to only allow that. Other alternatives include Authy, FreeOTP(I use this one)
* Physical token
* Email 

Note, I do not recommend SMS for MFA because phone numbers can be compromised more easily than the other MFA methods. The most prominent vulnerability with SMS is that of a "SIM Swap" attack in which a phone number is ported to a new service provider by a fraudster. 
[Wikipedia - SIM Swap Scam](https://en.wikipedia.org/wiki/SIM_swap_scam)
[So Hey You Should Stop Using Texts for Two-Factor Authentication](https://www.wired.com/2016/06/hey-stop-using-texts-two-factor-authentication/)

### Recovery Code
If your MFA does not work, such as if you were using an authenticator app on your phone and you lost your phone, then you can use your password managers recovery code to regain access to your account. it is essential that you write down your recovery codes and  keep them stored in a safe physical location, such as a physical vault.

## Important Password Manager Features

Most password managers have the feature to audit your passwords for best practises, such as whether the password is complex enough or if the website was compromised.

### Detecting Insecure Passwords

Run the following reports on your password manager and fix any issues found.

1. Reused Passwords Report
* If a service that you use is compromised, reusing the same password elsewhere can allow hackers to easily gain access to more of your online accounts. You should use a unique password for every account or service.

2. Weak Passwords Report
* Weak passwords can easily be guessed by hackers and automated tools that are used to crack passwords. The Bitwarden password generator can help you create strong passwords.

3. Unsecured Websites Report
* Using unsecured websites with the http:// scheme can be dangerous. If the website allows, you should always access it using the https:// scheme so that your connection is encrypted.

4. Inactive 2FA Report
* Two-factor authentication (2FA) is an important security setting that helps secure your accounts. If the website offers it, you should always enable two-factor authentication.


### Detecting Compromised Accounts 

Certain password managers have the ability to run a report on which accounts of yours have been breached. I suggest running the following reports on your password manager:

1. Exposed Passwords Report 
* Exposed passwords are passwords that have been uncovered in known data breaches that were released publicly or sold on the dark web by hackers.

2. Data Breach Report
* A "breach" is an incident where a site's data has been illegally accessed by hackers and then released publicly. Review the types of data that were compromised (email addresses, passwords, credit cards etc.) and take appropriate action, such as changing passwords.

3. Financial Statements
* Although not part of the password manager, I suggest checking your financial statements regularly(or better yet, enable notifications for every purchase). The credit card companies do their best to detect fraud, however if the fraudulent purchase might fit the characteristics of a legitimate purchase and not be considered a fraudulent purchase at first. This might happen, for instance, if your inactive Netflix account were compromised and the malicious person reactivated the account for the premium service.
* By validating all your purchases, any instances of a compromised account with your saved payment details will be caught early and prevent any losses. 


### Auto-Fill Capabilities
I highly suggest to NOT use any autofill features used in password managers as there are working proofs of concepts that would exploit this feature to exfiltrate the credentials.
[Password Managers: Attacks and Defenses](https://www.cs.columbia.edu/~suman/docs/suman_pwdmgr.pdf)


### Final Words

It is becoming increasingly difficult to ensure that all our passwords are secure. A password manager will help make sure that Mr X will not be able to compromise your accounts.




