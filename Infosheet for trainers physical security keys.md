# Infosheet: Physical security keys
(A guide for digital security trainers)

**Note**: This infosheet assumes you understand 2-factor authentication (2FA) and uses various related terms. To brush up on 2FA, good articles can be found online or try these from Okta or TechTarget.

**A physical security key** looks a little bit like a flash drive. It can typically communicate with your devices through USB-A, USB-C, or wireless technologies such as Bluetooth or NFC. There are two main things you can do with a physical security key:

* You could use it as a 2nd login factor in addition to your account password, instead of obtaining codes e.g. from an authenticator app (known as U2F, short for Universal Second Factor)
* You could use it to create and authenticate passkeys, also known as ‘passwordless login’ (known as FIDO2 or WebAuthn)

Physical security keys which support passkeys (see separate infosheet on passkeys) first began to be manufactured in 2018, while passkeys themselves only became widely available in 2022. Not all physical security keys will support the FIDO2/WebAuthn standard, but all can be used as a U2F key.

This infosheet will focus on how we can use physical security keys that support U2F. We’ve created a second infosheet on passkeys which will cover how to use physical
security keys with FIDO2 passkeys/passwordless logins.

*Note for Trainers*: Occasionally, physical security keys are also referred to as FIDO keys, named after an organization that promotes web authentication standards. We typically discourage this naming, since FIDO also oversees passkeys. Similarly, you may hear these referred to as YubiKeys, which is the brand of one leading vendor of physical security keys.

## Why do we promote physical security keys?

Physical security keys have one major advantage over authenticator or SMS-based methods of two-factor authentication: they are very resistant to phishing attacks.

An attacker could create a phishing website that asks for a targeted user’s password and authenticator app or SMS code, and then instantly enters the two into the real website,thereby gaining access to the user’s account before their authenticator app code expires.

A physical security key protects against this because it sends a code that is tied to the webpage on which it was registered. A fake website that tries to serve as an intermediary between the user and a real website will receive a different code - one that it will not be able to pass on to the real website. This is because phishing sites have different domain names than their real counterparts, which the security key mechanism will detect.

For this reason, many newsrooms and other institutions that are at high risk of sophisticated phishing attacks require team members to use either a physical security key or passkey to log in. Once they do that, it's practically impossible to access the accounts through phishing attacks.

## How do you set up and use physical security keys as a second factor?

Platforms which support physical security keys (U2F) as a second factor of authentication will display this option in the account security section for 2FA settings. Once you have set up your accounts to use a physical security key, you will log in the usual way, by going to your account's login page and entering your username and password. Following this, the website will ask you to insert the physical security key you registered with your account into your device's USB port and touch the button on the key (it's okay if the key is already in the port; you typically do not need to remove it and put it in again). Once you've done that, you should be logged in!

## What else should I know about managing my keys?

Platforms will also have options to remove a security key, and it's crucial to do so if you lose or give away your key. This will prevent people who have gotten your key from using it as a form of two-factor authentication for accounts you control (however, even if somebody were to temporarily access or steal your key, they would still not be able to do anything without your password).

It’s a good idea to have at least two physical security keys: a main one and a backup. That will allow you to still maintain access to your account if you lose or damage your main key. Most sites that support physical security keys allow you to add multiple keys; for those that do not, we strongly recommend generating and downloading account recovery codes and keeping those in a safe place in case you ever lose your physical security key.

You can use a single physical security key for as many accounts as you would like. And good news: the websites you use it with will not be able to figure out where else you might be using it. If, for example, you use the same key for Gmail and Facebook, then Facebook's parent company will not be able to see that you use Gmail—or view your login information there—based on your security key alone.

## Note for Trainers

The phishing resistance in physical security keys is a result of the keys being cryptographically tied to the website where they are registered.

When a website requests authentication through a physical security key, it will send a secret series of characters to the key, which combines those characters with some secrets stored on the key itself and sends back the result to the website. That website then checks this code once again.

This means that, if a phishing site tried to send a request to a physical security key and then forward the result it receives from the code to the real webpage, the real webpage would not accept this result, since it was calculated using the secret key of the phishing site rather, than that of the real webpage.

## Note for Trainers

Physical security keys typically contain a few additional security mechanisms. You always need to physically touch a button on the key to authenticate: this prevents bots or other automations from trying to study your key's contents.

The keys are also designed to be impossible to duplicate: even if somebody got hold of your key, in principle they should not be able to reproduce its secrets (in practice, vulnerabilities have been discovered at various points of time which would allow an attacker with sophisticated lab equipment to obtain a private key from certain vulnerable devices, for instance Yubikeys prior to version 5.70).

Finally, the keys also contain a counter. Every time the key's button is pressed, the counter goes up by one. The website you log in to keeps track of that counter every time you use a security key. If you tried to log in using a counter that is lower than the last request the website received from you, it should assume that someone intercepted your communication and refuse to log you in.

*This infosheet was developed in October 2024, for Internews partners and fellows delivering digital security training activities. You are welcome to adapt, edit, or translate this sheet based on your training needs.*

The above content has been released under the [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license