# Infosheet: Enhancing privacy by disabling mobile advertising IDs

Mobile advertising IDs are unique identifiers accessible to apps on both Android and iOS devices. They allow app developers and their advertisers to track users over multiple apps, allowing them to show more targeted ads. They have privacy implications, especially for high-risk individuals, and could be used to track the mobile phone’s location. Thankfully, it is possible to disable them.

On iOS, the ID is called Identifier for Advertisers (IDFA), whereas the Android equivalent is called Google Advertising ID (GAID). These names may change in the future.

Both kinds of advertising IDs are random sequences of letters and numbers that don’t contain any information identifying the user of the device. Those IDs will, however, often be combined with location data and other sensitive information that apps could have been given access to.

## Can you give a real-world example?

In a [real-world example](https://www.vice.com/en/article/muslim-app-location-data-salaat-first/), someone may have installed a religious prayer app that accesses their device’s location. This app includes functionality to display ads, which means it has access to the device’s location data, which it can then sell to data brokers – companies that make money by selling personal information. Any customer of the data broker would be able to see which user of the app was where, and at what time. It’s not just advertisers who buy such data; governments, militaries, and regulators frequently do so as well.

While the users on whom a data broker collected information might initially be anonymized, it’s often possible to determine who they are after capturing enough location data points–especially if data brokers and their customers have access to data from multiple apps.

If for example a weather app, a prayer app, a taxi app, and an app tracking pollution all have access to your location data and share this information with data brokers, then data brokers could use your advertising ID to associate all this data with a single device. And, since most of our movements are rather unique (you might be the only person at your office to frequent a particular restaurant), it’s reasonably easy to use this data to identify individuals.

## What can I do about this?

Thankfully, advertising IDs can be turned off!

If you are using a device with **Android version 12 and higher**, you can do this through the Settings app, by going to Privacy -> Ads and then choosing “Delete advertising ID”. This permanently deletes the advertising ID. Any app trying to access it will be given an empty response.

On **iOS devices**, in the Settings app, you can go to Privacy & Security -> Tracking and then turn off “Allow apps to Request to Track”. Here you can also see which apps have previously been granted this permission and you can revoke it for them.

While most privacy improvements come with downsides, disabling advertising IDs has almost none–unless a person prefers seeing mobile ads that are more targeted to them.

## Learn More

For more information about Mobile Advertising IDs, be sure to consult the below guide. Published by the Electronic Frontier Foundation (EFF), it gives additional background information on advertising IDs, and shows you how to disable them on older Android devices. It also provides some information on others kinds of tracking.
[How to Disable Ad ID Tracking on iOS and Android, and Why You Should Do It Now](https://www.eff.org/deeplinks/2022/05/how-disable-ad-id-tracking-ios-and-android-and-why-you-should-do-it-now)
