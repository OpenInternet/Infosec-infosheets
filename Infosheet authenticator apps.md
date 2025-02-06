# Infosheet: Authenticator Apps

Authenticator apps provide a second factor in two-factor (or two-step, or multi-factor) authentication, and are often used after someone logs in with a password. That way, even if an adversary managed to somehow capture your password (maybe they found it in a leaked passwords database or looked over your shoulder while you were typing it), they would not be able to log in without this second factor. This significantly reduces the chances of an adversary taking over your account.

## How authenticator apps work

Most authenticator apps include time-based one-time passwords (TOTP). For each account the app is set up for, a six-digit code is shown, which changes at regular intervals, every 30 or 60 seconds. When a service (such as an email provider or social media platform) needs to check your identity – for example, when you log in to your account using a new device or from a new location – it might ask you to enter a current code from your authenticator app in addition to your password, and will only log you in upon receiving the correct password-code combination.
Under the hood, an authenticator app contains a ‘secret’ (called a ‘seed’) that only it and the service it is used for have access to. That secret is used to generate and verify the ever changing six-digit codes. Cryptography is used that makes it impossible to predict the codes that are shown in the app.

There are various kinds of authenticator apps, such as Google Authenticator, Authy and Duo Mobile. Microsoft also has its own authenticator app that can be used both for TOTP and to securely login to Microsoft services. In the latter case, the user has previously logged into the app and merely confirms the login by entering a two-digit code presented by Microsoft during
the login process.

When you first add a new account into your authenticator app, the service (for example your email provider) will typically show you a QR code, which you scan through your authenticator app. The service will then display a six-digit code, which you will need to type into your authenticator app. After this, the authenticator app is set up for this account.

## Backups!

To prevent being locked out of one’s account in case a device is lost, stolen or broken, it is strongly recommended to back up the app and the accounts stored therein.

Many platforms that support 2FA – regardless of the type of 2FA they support – allow for ‘backup codes’ to be downloaded. They are designed for situations in which you remember your password but cannot access app-based or security key-based 2FA (for example, perhaps you lost a device or accidentally uninstalled your authenticator app from your phone).

You can print the backup codes and store them in a safe place. You can also store them in a password manager. However, it is important that you store them in a place that you have relatively easy access to in case your regular 2FA doesn’t work, for example because your phone is lost or stolen.

At the same time, having easily accessible backup codes needs to be balanced with the risk of someone obtaining them and thus being able to login to your account. In particular, if backup codes are stored within a password manager together with the password of the account they are used for, someone with access to the password manager has everything they need to login to the account.

*It is good to keep in mind that backup codes can be phished in the same way that TOTP can be.*

If the authenticator app has login functionality (such as with Google’s and Microsoft’s authenticator apps), backups are typically done automatically – though it is important to confirm this. Of course, the account to which the data is backed up to should itself have strong authentication! The issue with this approach is that you might need a two-factor code to log in to the authenticator app – which contains your backups – in the first place. For this reason, if you only have one device on which all your app-based codes are synced, we recommend keeping a copy of your backup codes (and instructions on how to log in to your password manager or access key passwords) in a different, safe place.

## Advantages and downsides of app-based authentication

App-based authentication is much stronger than password-only authentication, and also more secure than SMS-based two-factor authentication. It does, however, share a weakness with the latter: the risk of real-time adversary-in-the-middle phishing attacks. In this kind of attack, a phishing page doesn’t merely collect login details but also attempts to use them to login to the targeted service in real time. If this service asks for a one-time password – either provided through SMS or through an authenticator app – the phishing page asks the user for this code and then enters this into the real site. Physical security keys and passkeys do not have this weakness, and are thus recommended (as being more secure) for high-risk users.

*This infosheet was developed in October 2024 for Internews partners and fellows delivering digital security training activities. You are welcome to adapt, edit, or translate this sheet based on your training needs.*

The above content has been released under the [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license