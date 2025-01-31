---
type: rule
title: Security - Do you have a strict password security policy?
uri: have-a-strict-password-security-policy
authors:
  - title: Stanley Sidik
    url: https://ssw.com.au/people/stanley-sidik
  - title: Kiki Biancatti
    url: https://ssw.com.au/people/kaique-biancatti
    img: https://raw.githubusercontent.com/SSWConsulting/SSW.People.Profiles/main/Kaique-Biancatti/Images/Kaique-Biancatti-Profile.jpg
  - title: Adam Cogan
    url: https://ssw.com.au/people/adam-cogan
related:
  - do-you-have-mfa-multi-factor-authentication-enabled
redirects:
  - do-you-have-a-strict-password-security-policy
created: 2017-07-10T20:55:19.000Z
archivedreason: null
guid: 4bc01f63-9631-4dec-ab28-aa17d89387d3
---
We recommend enforcing policies based on reputable regulatory organizations (e.g. NIST, ACSC) latest recommendations.

<!--endintro-->

::: good  
![Figure: Good example - Active Directory settings based on latest security recommendations](adnewpasspolicy.jpg)
:::

When passwords have to be changed they should meet the following complexity requirements:

* **Ignore password complexity (numbers, special characters, spaces) but require longer passwords** - E.g. require 16 characters length minimum, without special characters or numbers
* **Longer password history remembered** - E.g. cannot use the last 10 passwords you already used
* **Blocking of common password and words** – E.g. via Azure AD Password Protection (https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-password-ban-bad-on-premises)
* **Use of MFA (Multi Factor Authentication) everywhere possible** - https://www.ssw.com.au/rules/do-you-have-mfa-multi-factor-authentication-enabled
* **Use a password manager**
* **Use different passwords for every service** – E.g. different passwords for your Outlook, Facebook…

We also enforce a lockout policy so if a user gets their password wrong 5 times, their account will be locked out for 15 minutes.

Longer passphrases are better than passwords, they are even more difficult to crack than complex passwords https://www.zdnet.com/article/fbi-recommends-passphrases-over-password-complexity/

::: bad
Bad Example: Requiring users to change their passwords e.g. every 180 days does not improve security. If you already have a strong password (as above) and a second factor of authentication (e.g. MFA) changing it does very little to make you more secure. Generally, you should change your password only when you believe it has been compromised.
:::