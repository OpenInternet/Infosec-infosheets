
# Messenger hardening guides

## Enable two-step verification/ two-factor authentication

As we mentioned in our guide on [messenger takeovers](Infosheet messenger takeover attacks.md), someone who manages to intercept SMS messages sent to your account--or tricks you into sending them a six-digit code--will be able to take over your WhatsApp, Signal, or Telegram account. Fortunately, it's easy to set an additional password without which you cannot register the account on a new device. We strongly encourage enabling this feature.

### How to enable this feature

[WhatsApp](https://faq.whatsapp.com/1278661612895630) \
[Signal](https://support.signal.org/hc/en-us/articles/360007059792-Signal-PIN#manage_registration_lock) (enable PIN and registration lock) \
[Telegram](https://telegram.org/blog/sessions-and-2-step-verification)



## Disappearing messages

You can enable disappearing messages on your chats. Once you do so, messages will be automatically removed from your devices as well as those of your interlocutors. Disappearing messages work on a timer (for example, they might automatically get wiped after 24 hours or a week). This reduces the chances that message contents will be leaked if, for example, a device was lost or stolen while unlocked or broken into.

In Signal, the timer begins on the sender's device when the message is sent and on the recipient's device when the message is opened. In WhatsApp, the timer begins on both the sender's and recipient's devices after the message is sent.

Telegram _only_ supports automatic disappearing messages on secret chats, not standard chats or groupchats.

### How to enable this feature

[WhatsApp](https://faq.whatsapp.com/673193694148537) \
[Signal](https://support.signal.org/hc/en-us/articles/360007320771-Set-and-manage-disappearing-messages) \
[Telegram](https://www.howtogeek.com/710073/how-to-send-disappearing-messages-in-telegram/) (only on secret chats, not on groupchats)


## Signal usernames and phone number privacy

Signal has recently introduced _usernames_, which allow you to hide your phone number from people you talk to. This is particularly useful for those who would prefer not to reveal their real-life identity, or are concerned about targeted harassment. 

### How to enable this feature

[Signal](https://support.signal.org/hc/en-us/articles/6712070553754-Phone-Number-Privacy-and-Usernames)


## Security notifications

When you see a _security notification_ on your device, it means that something changed about the Signal or WhatsApp installation of the person you're talking to (or are in a groupchat with). In most cases, it means that they reinstalled Signal or WhatsApp or has a new device. It could, however, also mean that someone else has taken over their account and registered it on a new device. If you see a security notification, it's a good idea to reach out to the person and verify their identity, for example by asking what you chatted about at the last lunch you had together.

For more information, check out our guide to [messenger takeover attacks](Infosheet messenger takeover attacks.md).

Signal shows security notifications by default. In order to see them on WhatsApp, you need to enable them manually.

### How to enable this feature

[Signal](https://support.signal.org/hc/en-us/articles/360007060632-What-is-a-safety-number-and-why-do-I-see-that-it-changed) \
[WhatsApp](https://faq.whatsapp.com/1524220618005378/)

## Location privacy during phone calls and video chats

When you call somebody over a messenger, the call go directly from your phone or that of the recipient. The latter is typically easier and leads to higher quality calls. Since you connect directly to someone else's device, you will inevitably need to share the IP address from which you are calling. IP addresses can be correlated with your location (or alternatively, reveal the fact that you're using a VPN), so some at risk individuals would prefer to hide them when calling others through a messenger. Thankfully, WhatsApp, Signal, and Telegram all offer the option to relay all calls through their servers. While possibly reducing call quality, it will hide your IP address from whoever you are talking to.

### How to enable this feature

[WhatsApp](https://faq.whatsapp.com/2635108359972899) \
**Signal:** Go to your settings ➡️ Calls ➡️ Always relay calls \
**Telegram:** Go to your settings ➡️ Privacy and Security ➡️ Calls ➡️ Peer-to-peer

## Encrypted backups

WhatsApp allows you to back up your conversations to Google Drive or iCloud. That way, even if your phone was lost, broken, or stolen, you could still easily restore an archive of your chats. As an additional protection, you can also encrypt those backups with a special password: that way, if anyone were to gain access to the account where those backups are stored, they would be unable to read their content without the password.

Do note that you will not be able to access the data stored in the backup without the password. As such, make sure to store it in a safe place.

### How to enable this feature

[WhatsApp](https://faq.whatsapp.com/490592613091019)


----


The above content has been released under the [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license
