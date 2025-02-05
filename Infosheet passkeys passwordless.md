# Infosheet: Passkeys (or ‘passwordless’ login)

In recent years, a new login standard has emerged that is commonly referred to as passkeys or ‘passwordless’ login. (The formal name for the standard is WebAuthn or FIDO2, but you’ll rarely encounter those terms). They aim to solve the shortcomings of other forms of two-factor authentication (2FA), which were either vulnerable to phishing attacks (such as those involving codes being sent by SMS or email) or relied on an easy-to-lose physical USB key. Passkeys are also significantly easier to use than other existing 2FA methods, as they securely log in a user without needing them to type in a password.

## How do passkeys work, anyway?

A unique passkey is created for each service/platform and can be stored in your desktop or mobile operating system (which relies on a special security hardware chip to protect the key), a physical security key,[^1] a web browser, or a password manager. Essentially it is a private key—or a secret sequence of bytes that only your device knows, with a matching public key stored by the platform. A platform or service that wants to authenticate you using passkeys will send a brief message to your device, where a passkey management service securely retrieves the private keys, signs the message, and sends it back. The platform can then see that the response was created with the valid private key, by confirming it against the stored public key.

Logging in using passkeys involves responding to a prompt sent to your device—this may be the same device you’re logging in from, or it may be a different device—asking you to confirm the login. Often this involves using a fingerprint, FaceID, or entering a device passcode to provide an additional, user-friendly layer of verification. In the case where you wish to use a physical security key to store a passkey, you will be asked to insert or tap the key to your device.

Passkeys tend to work smoothly. They automatically handle all the authentication messages sent between devices and the calculations that underpin the authentication process. This process is so simple that many people already use passkeys without even realizing it! This simplicity can sometimes prove challenging during trainings: we are accustomed to more complex security mechanisms (such as long, complex passwords and physical security keys), making it hard to believe that a simple prompt on your device can replace them. Still, it is important to remember that, under the hood, passkeys perform very strong authentication.

## Passkeys are phishing-resistant!

Just like physical security keys, a passkey is tied to the service where it was registered. This means that it is not possible for an adversary to trick you into using your passkey on a fake website and then relay this information to the real website on your behalf (known as an adversary-in-the-middle attack). A passkey would simply fail when used on the wrong website, since the fake website uses a different domain from the real one, even if it is a cleverly-created lookalike.

## Testing and setting up passkeys

Many online platforms have rolled out passkeys, and support is expected to become more widespread across the web. Still, passkeys are relatively untested and poorly understood by most users. High-risk groups, particularly those with unusual set-ups that may consist of multiple devices that they don’t always have access to, and who face increased physical threats or threats of duress, may need special consideration. In addition, individuals with older hardware or intermittent network or Bluetooth functionality may have difficulty with passkeys.

Because the technology has been rolled out only recently (since 2022) and often works relatively seamlessly, users often have a hard time understanding what is happening or identifying where their passkeys are stored. Similarly, while some services just request passkeys, others might still require the user to type in a username and password and only later authenticate through a passkey. The standards body responsible for rolling out passkeys has not yet published standards on how to back them up or move them between devices. Currently, the recommendation is to create a separate passkey for every device you own, or alternatively synchronize them across all devices through a password manager. We also recommend creating a backup authentication method, such as a security key that uses U2F, in case the devices on which you store your passkeys are lost or damaged.

For these reasons, we recommend everyone to experiment with passkeys on sites designed for testing them — such as [https://www.passkeys.io](https://www.passkeys.io) or [https://webauthn.io](https://webauthn.io) — before trying them on active accounts.

*This infosheet was developed in October 2024, for Internews partners and fellows delivering digital security training activities. You are welcome to adapt, edit, or translate this sheet based on your training needs.*

[^1]: Not all physical security keys can store passkeys. Those that do are usually referred to as FIDO2 security keys. They usually support both passkeys and Universal 2nd Factor (U2F) logins.