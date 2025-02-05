# Infosheet: messenger takeover attacks

Many messenger applications – including WhatsApp, Signal, and Telegram – use our phone number for both registration and authentication purposes\*. If we need to re-register our account on a new phone, we don’t always have access to our old phone (for example, it might have been lost, stolen, or damaged). However, during the re-registration process, the messenger will still send a re-registration code via SMS to the phone number the account was previously registered on. This is because the messenger uses a phone number as an authentication mechanism and assumes that, if you can receive and read SMS messages from a phone number, then you must be its owner.

**An adversary who manages to obtain your re-registration code could take over your account**. They can then see all future messages you receive and send messages on your behalf (your contacts will, however, see that your security code changed). They can also fully lock you out of your account by deciding which devices (such as your laptop) have access to it. Finally, adversaries who take over your account this way could figure out what groups you are in (if you use WhatsApp, Signal, or Telegram) and your past message history (if you use Telegram and only for conversations which aren’t secure chats).

**SMS should be considered insecure**. An attack on a company sending out SMS messages resulted in a prominent journalist’s Signal account being taken over. It’s also common to see social engineering attacks where someone sends you a message like “hey, this is my old number. Forgot to change it. A six-digit code was sent to me – could you share it?” In retrospect, those are obvious attempts to capture registration codes, but adversaries constantly improve their tactics. Some trick people into thinking that they can use messengers to register for prize draws and then ask them for registration codes.

Training people never to share registration SMS codes is great – but imperfect. An attacker can try many times to trick you. You just need to fall for it once; adversaries could reach you when you’re feeling tired, ill, or overwhelmed. Attackers could also try to directly capture SMS codes without your knowledge if they can access or break into telecom infrastructure.

## Protect your accounts:

Every major messenger offers the possibility of enabling a password or PIN that must be entered to register your number on a new device, and we strongly recommend enabling this feature. This can be done in [Signal](https://support.signal.org/hc/en-us/articles/360007059792-Signal-PIN) (enable both the PIN and registration lock), [WhatsApp](https://faq.whatsapp.com/506595211487528), [Telegram](https://support.signal.org/hc/en-us/articles/360007059792-Signal-PIN), and many other messengers. We strongly recommend all users enable this second verification step and save their PIN or password in a safe place, such as a secure password manager.

If you lose your PIN or password for Signal or WhatsApp, you will need to wait seven days to register your number on a new device. If an adversary stole your SMS code and waited for that long, they too could take over your account. To help protect against this, be sure to always open each of your messenger applications at least twice a week (and see if you don’t encounter a security message right after opening it) to ensure that nobody else is trying to gain access to your account.



\* While both Signal and Telegram offer the option of hiding your phone number, this just means that other users you message can’t see your number. The services can still use your number to authenticate your account on a new device. Signal now allows you to register on new devices with the PIN alone, with no SMS codes.

*This infosheet was developed in December 2024, for Internews partners and fellows delivering digital security training activities. You are welcome to adapt, edit, or translate this sheet based on your training needs.*