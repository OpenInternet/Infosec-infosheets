# Infosheet: Identity management

***STILL IN BETA, NOT YET PRODUCTION READY***

Sometimes, it's not possible for us to safely do all of our work under a single name, and we might need to create separate identities. An activist supporting at-risk individuals in a repressive country, for example, might be using one identity for this type of work, and another for standard social and professional interactions.

Some people willingly and openly use those different identities. For others, though, it's important that the different identities cannot be easily tied together. We've listed a few steps you could take to keep your different identities safely apart:

## Map out all identities

To secure something, you first need to know about it. Make a list of all the different accounts and services each identity uses: those could include email addresses, social media accounts, websites, and more.
Make sure that each of those accounts has a long, unique password and two-factor authentication (ideally with physical security keys or passkeys.) 

## Each identity should have its own e-mail address

Social media accounts, and other online services, are typically linked to email addresses. While websites generally do not reveal what email address is associated with which account, such information could occasionally leak out. The service itself could be poorly configured or be at the receiving end of a cyberattack; it could also reveal email addresses through a poorly designed password recovery form. For this reason, it's important that you create a separate email address for each identity, and register all social network accounts and the like to it.

## Beware of real name policies

Some social media services require you to use your real (passport) name on the account, and might block your accounts if you do not adhere to this. This policy is fundamentally incompatible with any security-aware identity and persona management. There are, unfortunately, no easy ways to get around it except for being ready for the account to be blocked and relying more on social networks which do not have real name policies.

## Think of other ways in which your identities could be correlated

### Posting times and patterns

If all of your accounts post during the same timeslot during the day, then somebody who is closely watching them could guess that they are somewhat related. Similarly, if one of your accounts announces that it's off on a business trip, and the others either go silent or start posting from what looks like a different timezone, this could also suggest that those accounts are somehow related. Inconsistent posting times can prove very helpful here.

### Photo metadata

Most photos contain metadata, which could include the model of the camera that took the photo, the time the photo was taken, and possibly the photo's location. If your different accounts upload photos taken by the same camera, then metadata could be used to connect them. There are times when metadata is very important—for example when you are collecting evidence and want to preserve a chain of custody—but at other moments it can be a problem.
Some social networks might automatically remove metadata, but since different services have different settings, it's best to manually clear it prior to upload. One of the easiest ways of removing image metadata is by sending the image to yourself on Signal, and re-downloading it. The downloaded image should have had all of its metadata cleared (in addition to being compressed). Open the downloaded image in a file explorer or image viewer to check if all the metadata has been removed.

### Social networks and online communities

Social media platforms can be a fantastic tool to connect and share with each other, and also spread your message. It can also be important for community organizing. Still, you must be careful about whom you follow or add to groups: your different identities should not be publicly linked to the same people or groups. Similarly, be careful of whom you trust, and verify all groups or groupchats with trusted sources.

### Use of language/content

We all have our favourite words and phrases (this piece's author enjoys overusing the em dash), and unique language or phrases can tell us apart. It might be a good idea for different identities to use slightly different tones in their writing. Generally be mindful of the content you share. Although you may be using different identities, unconsciously, the same personal experience narrative could be similiar and this may expose you to an alert attacker who may be searching for clues.

### Domain names

Anyone who registers a domain must give their details, such as name and address, to their registrar. While not always enforced, giving fake details could lead to the registration being suspended. Sometimes, the details you give to the registrar could be published and visible through tools such as RDAP or WHOIS. To ensure that nobody (except for the registrar) can see your details, enable RDAP/WHOIS privacy. Many registrars have already turned this on by default, though some might charge an extra fee for it.
