
# Infosheet: weaknesses in SMS

Using **SMS-based two-factor authentication (2FA)**, a user logs into their account by entering their username and password, and then enters an additional Time-based One-Time Password (TOTP), which is delivered to them via SMS or text message. Though this type of account security is certainly better than not having any two-factor authentication (2FA) at all, SMS-based 2FA is widely considered to be one of the weakest kinds of 2FA.

Some of its weaknesses – such as the fact that it is vulnerable to 2FA-aware phishing – are shared with other forms of TOTP 2FA, such as authenticator apps. Similarly, relying on any type of 2FA (including SMS-based 2FA) could result in malicious apps gaining access to your accounts through something called OAUTH or Open Authorization (which is an open standard that allows users to grant third-party applications access to their information, without actually having to share their passwords).

However, beyond these “shared” vulnerabilities, there are a number of things that make SMS-based 2FA particularly vulnerable to attacks – and it should be noted that even if SMS-based 2FA isn’t used, there may still be services that rely on SMS access that are thus similarly vulnerable to the same weaknesses.

## Weakness #1: Physical access to a phone – through theft, loss, seizure, or a relationship between the adversary and their target.

Though access to an unlocked device grants an adversary access to authenticator apps, even on a locked device, SMS notifications (such as those containing a One-Time Password) still show up on the screen by default.

Luckily, this can be turned off on Android devices in the Settings app, by going to Notifications and then disabling ‘notifications on lock screen’. On iOS, this can also be set on a per-app basis in the Notifications section of the Settings menu.

## Weakness #2: Physical access to a SIM card.

An attacker who takes a SIM card out of a phone and puts it into another phone will alsobe able to receive SMS messages, without even knowing the password to the lockeddevice. Some phone providers mitigate this threat by protecting their SIM cards with aPIN code that needs to be entered before the SIM card can be used.

## Weakness #3: SIM swapping.

If a SIM card is lost or stolen, a mobile phone provider is able to replace and/or grant a new SIM card with the same mobile number. “SIM swapping” is the practice by which an
adversary uses social engineering to convince a phone company to provide them with a new SIM card for a target account. This type of attack is frequently [used to target well-known activists](https://www.engadget.com/2016-06-10-hacker-hijacks-deray-by-redirecting-his-verizon-phone-number.html), journalists, and investors.
SIM swapping does take a certain amount of work on behalf of the adversary, who willneed to know some of the target’s personal information, but it has been shown to beeffective in more targeted attacks.

Some phone providers allow you to set a password or code that anyone who wants torequest a new SIM card will need to show. If this security option is available, it is stronglyrecommend that high-risk individuals enable it. That way, attackers who do not know that password or code will not be able to easily manipulate the telecom company intogranting them a new SIM that has access to your account. Of course, it is up to the phone provider to ensure the correct procedures are being followed, and that no new SIM cards are provided without the PIN or password.
Sometimes people express concern about a similar type of attack called **SIM cloning**, where an existing SIM card is cloned to create a second SIM card that can receive thesame messages. Early SIM cards were indeed vulnerable to SIM cloning, but for modernSIM cards, cloning is beyond the capabilities of even the most advanced adversaries.

## Weakness #4: SS7 Protocol.

Another way an adversary can obtain access to SMS messages is through [weaknesses](https://www.eff.org/deeplinks/2024/07/eff-fcc-ss7-vulnerable-and-telecoms-must-acknowledge) in the SS7 protocol. This is the protocol that ensures SMS messages can be sent and received while roaming on a different mobile network, for example when traveling abroad.
SS7 is an old protocol that wasn’t built with security in mind (and unlike most other messengers isn’t end-to-end encrypted), but governments, cyber mercenaries (companies that hack on behalf of others, typically governments) and cybercriminalswith the right means and/or connections have been known to use weaknesses in SS7to intercept SMS data. Moreover, the same weaknesses in SS7 (as well as some in the newer Diameter protocol) can also be used to track the location of a mobile phone by determining whatcell tower(s) it connects to. Unfortunately, there is no way for someone to detect or prevent SS7 abuse.

## Weakness #5: Providers.

Finally, in some cases the providers that send SMS messages on companies’ behalfare hackable and/or corrupt, allowing for adversaries with the right means and/or contacts to intercept SMS messages in real time as they are being sent. It should benoted that platforms often use local providers in the country to send SMS on their behalf. Platforms may be unable or unwilling to check the security of these providers—which could lead to user’s SMS messages (and any accounts relying on SMS-based 2FA) to be at risk.

## Conclusion

If the service you're signed up for only uses SMS for 2FA, then by all means use it. But if it offers alternative methods, such as authenticator apps or ideally physical security keys or passkeys, then we recommend using those instead and turning off SMS for 2FA. If you do so, make sure to also print off backup codes or set up more than one method of 2FA so that you do not accidentally lock yourself out of your account—if, for example, you lose a device.

*This infosheet was developed in December 2024 for Internews partners and fellows delivering digital security training activities. You are welcome to adapt, edit, ortranslate this sheet based on your training needs.*

The above content has been released under the [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license