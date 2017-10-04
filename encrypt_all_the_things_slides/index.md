<img src="http://blog.serverfault.com/files/2016/02/encrypt-all-the-things1.png" width=30%/>

**... but don't forget your keys.**

*(Digital Privacy & Security for Researchers)*

A primer for the "Attacks on Encryption" event

5 October, 2017, Brisbane

Brenda Moon & Felix Victor Münch

<font size=0.5>image: http://blog.serverfault.com/files/2016/02/encrypt-all-the-things1.png
(based on original by http://hyperboleandahalf.blogspot.com.au/)
</font>

----

<font size=3>
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a></br>
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.</font>

---

# Why are we here?

Note:
TODO for Brenda, introduction

----

# worst case scenarios

----

## weak password reuse

your standard password appears in a major data breach – and suddenly your devices are wiped

Note:
haveibeenpwned.com

----

## revealing IP address

researching in extremist bulletin boards/social networks
getting harassed in your neighbourhood afterwards

----

## unencrypted communication

communication with protesters in an authoritarian surveillance state via iMessage but message gets accidentially sent via SMS service

----

## unencrypted devices

interview in country oppressing the press with 'off-the-record' content on unencrypted Android phone gets confiscated at the airport before leaving the country

----

## Metadata retention

<img src='encrypt_all_the_things_slides/img/snitch_hunt.png' width="70%">

(http://www.abc.net.au/triplej/programs/hack/how-team-of-pre-teens-found-whisteblower-using-metadata/8113668)

Note:
* This is a privacy and security risk faced by everyone, not just researchers.
* The slide shows a news article about a realistic metadata game where a team of pre-teens identified a whistleblower in less than 2 hours

---

# Passwords

----

## Main risks

Especially when you've been pwned:

* common password (qwerty, 12345, monkey, love, ...)
* easy to guess (qwerty12345, your name, your birthday, your partners birthday, your postcode, )
* reuse of passwords
* storing password in an unsafe place (i.e. unencrypted and accessible from outside)
* forgetting your password

----

## Solution #1:

### Use a password manager

----

## We recommend

* KeePass, KeePassX, KeeWeb
    * Open source +
    * interoperable +
    * high reputation +
    * free +
    * not so convenient -
* 1Password
    * high reputation +
    * very convenient +
    * costs money -
    * closed source -

Note:
* links to all these are provided on the resources page at end of presentation

----

## Solution #2:

### Use 2-factor authentication

----

## We recommend

Use an app for 2 factor authentication (not SMS):

* [FreeOTP](https://freeotp.github.io/)
* [Google Authenticator (Android/iPhone/BlackBerry)](https://support.google.com/accounts/answer/1066447?hl=en)
* [Amazon AWS MFA (Android)](https://www.amazon.com/gp/product/B0061MU68M)
* [Authenticator (Windows Phone 7)](https://www.microsoft.com/en-us/store/p/authenticator/9wzdncrfj3rj)
* [Authy](https://www.authy.com/app/)

Note:
* links to these are provided in the resources section

---

# Researcher privacy

----

## Main risks

when researching on the internet:

* activity record (metadata) retention (by state/institution/ad networks)
    * by IP address (like a 'phone number' for your computer)
    * by browser cookies (like customer cards in shops, just for your browser)
* revealing of personal details to website owners
* other forms of browser finger printing

----

## Solution #1:

### Virtual Private Network (VPN) 'tunnel'

----

## We recommend

Choose a VPN service which:

* claims not to store activity records (hard to verify)
* uses OpenVPN
* has servers in safe jurisdictions
* not insert advertising into your browsing stream

[NordVPN](https://nordvpn.com/) and [Private Internet Access](https://www.privateinternetaccess.com/) both have a long term high reputation. [ProtonVPN](https://protonvpn.com/), made by the people behind ProtonMail, looks promising too.

Note:
Remember that if it's too cheap you might be paying in other ways.

----

## Solution #2:

### Tor Browser

----

## We recommend

Use TorBrowser for high risk research, not for everyday use.

Note: for high risk research get expert advice!

---

# Data storage

----

## Main risks

when storing data:

* unauthorised access to data, e.g. in the cloud
* unwanted access to devices, e.g. if stolen or taken by authorities
* data loss
* lost access

----

## Solution

----

# backup, backup, backup

3 independent copies

----

AND

----

![](http://blog.serverfault.com/files/2016/02/encrypt-all-the-things1.png)

**... but don't forget your keys.**
*(hint: use a password manager)*

----

## We recommend

* full device/disk/USB stick … encryption (mostly provided by OS)
* for files in the cloud:
    * [Cryptomator](https://cryptomator.org/)
    * [keybase](https://keybase.io/)
    * disk image encryption by your operating system

MAKE SURE YOU NEVER LOOSE YOUR KEYS OR PASSPHRASES!!! Or all will be lost.

---

# Communication

----

## Main risks

While transmitting sensitive information: the men in the middle

* your email/messaging provider or anybody who has hacked them or pretends to be them
* authorities who subpoena any of your communication providers
* others in open/untrusted WiFi

<img src="encrypt_all_the_things_slides/img/wifi-ios.png" class="fragment" width="40%">

Note:
* Email is like a postcard, even the post office can read it

----

## Solution #1:

### https

----

## We recommend

* check the address bar in your browser
![](encrypt_all_the_things_slides/img/2017-02-05%20at%201.41%20pm.png)

* [HTTPS Everywhere](https://www.eff.org/https-everywhere)


Examples for bad certificates: https://badssl.com/

Note: HTTPS Everywhere is a Firefox, Chrome, and Opera extension that encrypts your communications with many major websites

----

## Solution #2:

### PGP encryption

"Pretty Good Privacy"

----

## We recommend

* [keybase](https://keybase.io/)
* [GPGTools](https://gpgtools.org/) for MacOS
* [GPG4win](https://www.gpg4win.org/) for Windows
* [Enigmail for Thunderbird](https://www.enigmail.net/index.php/en/)
* email clients with GPG support

----

## Solution #3:

### Secure messenger / private messaging

----

## We recommend

* [Signal](https://whispersystems.org/)
* [keybase](https://https://keybase.io/)

---

# How to choose a tool?

----

## Things to consider

1. Open Source?
2. Reputation?
3. Independent security audit?
4. Will you actually use it?

---

# Where to from here?

At end of the presentation there is a list of all the software we've mentioned today and a list of useful websites for more information.

* Start using some of these tools!
* Use the suggested websites to become better informed!
* Keep your devices' software & application software up to date!
* Spread our workshop

----

## Get expert advice

Depending on the level of risk to you or your research participants you may need to seek advice from a security/privacy expert before you begin your research.

Note:
* Risks/Solutions are changing over time, so important to get current advice before you start your research.

---

# Questions?

---

# Resources

----

## Password manager

* 1Password https://1password.com/
* KeePass http://keepass.info/
* KeePassX https://www.keepassx.org/
* KeeWeb https://keeweb.info/

----

## 2-factor-authentication

* Amazon AWS MFA (Android) https://www.amazon.com/gp/product/B0061MU68M
* Authenticator (Windows Phone 7) https://www.microsoft.com/en-us/store/p/authenticator/9wzdncrfj3rj
* FreeOTP https://freeotp.github.io/
* Google Authenticator (Android/iPhone/BlackBerry) https://support.google.com/accounts/answer/1066447?hl=en
* Authy https://www.authy.com/app/

----

## Privacy

* Browser leaks https://browserleaks.com
* HTTPS Everywhere https://www.eff.org/https-everywhere
* NordVPN https://nordvpn.com/
* Private Internet Access https://www.privateinternetaccess.com/
* Tor Browser: https://www.torproject.org/projects/torbrowser.html.en

----

## file/device/communication encryption

* Cryptomator https://cryptomator.org/
* Enigmail for Thunderbird https://www.enigmail.net/index.php/en/
* GPGTools https://gpgtools.org/
* keybase https://keybase.io/
* Signal https://whispersystems.org/

----

## websites

* CryptoParty https://www.cryptoparty.in/
* Electronic Freedom Foundation (EFF)
  * Privacy https://www.eff.org/issues/privacy
  * Surveillance Self-Defense https://ssd.eff.org/
    This has overviews, tutorials, and detailed guides for specific situations.
* Snitch Hunt Game http://whistleblower.network/snitch/index.php
* Snitch Hunt news article http://www.abc.net.au/triplej/programs/hack/how-team-of-pre-teens-found-whisteblower-using-metadata/8113668
* Examples of Bad SSL certificates https://badssl.com/

---

# Glossary of terms

* browser cookies: like customer cards for your browser to store information about you that can be read by the website when you return
* encryption: making data practically unreadable without another piece of data (see keyfile) and/or password that's usually kept secret
* end-to-end encryption: encryption from a senders device to a recipient device without intermediaries being able to decrypt

----

# Glossary of terms

* https: HTTP over SSL https://en.wikipedia.org/wiki/HTTPS
* IP address: number to identify your computer/router to another computer, mostly a server serving you a website
* keyfile: think of it as a password, but in a file.
* metadata: activity records (https://twitter.com/Snowden/status/661305566967562240) or more detailed: https://ssd.eff.org/en/glossary/metadata
* ssl or tsl: Secure Sockets Layer / Transport Layer Security https://en.wikipedia.org/wiki/Transport_Layer_Security

---

![](https://abs.twimg.com/icons/apple-touch-icon-192x192.png)

[@brendam](https://twitter.com/brendam)
[@flxvctr](https://twitter.com/flxvctr)

QUT DMRC Fridays 25th August 2017

<font size=0.5><a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a></br>
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.</font>
