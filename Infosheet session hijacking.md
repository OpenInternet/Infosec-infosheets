# Infosheet: session hijacking

Session hijacking is an attack which grants an adversary temporary access to an account. While it typically doesn’t allow adversaries to make important changes (such as grant themselves long-term access to the account), it allows them to read and create content. From the user’s experience, a session hijack can appear very similar to an account hijack.

## Authentication cookies

Session hijacking involves stealing cookies, or small pieces of data that a website asks a browser to remember. For example, a website may ask the user to choose their preferred language and store that as a cookie. As the user visits the website again, their browser will send the cookie with the preferred language to the website, which now knows it without having to ask again. Cookies can also store information about which user is currently logged in. This is why, if you clear all cookies, you will need to re-enter your username, password, and 2FA code (or passkey) into all websites again–the website will have no way of remembering who you are.

If an adversary obtains a cookie that your browser uses for authentication (also known as a session cookie), they can impersonate you from their own computer by simply adding the session cookie to their browser, a process they can fully automate. By obtaining access to a session cookie, an adversary typically has the same access to the account that any logged-in user would have. Depending on the platform, this could mean access to sent and received emails or direct messages. They are also able to generate new content, such as sending emails or social media posts. While most online platforms have some defenses against adversaries logging in with stolen session cookies, skilled adversaries can sometimes overcome those defenses.

## How are cookies stolen, anyway?

In the past, session cookies could be easily stolen on public WiFi networks: communication between laptops and servers was not encrypted, and attackers could [easily](https://en.wikipedia.org/wiki/Firesheep) snoop on all communication, including cookies. Thankfully, the widespread adoption of HTTPS has made this type of attack infeasible and almost all websites can now be safely browsed on a public WiFi network.

Session cookies could also be stolen through malware or malicious extensions installed on a device. Many “too good to be true” browser extensions steal session cookies. High-risk individuals should be very wary when installing any kind of software onto their device, which includes browser extensions that customize their online experience. Those could be adding or removing content from websites they view, for example, or offering special features like automatic language translations or grammar checks. Users should also beware of browser extensions that require a great many permissions to activate. Cookies can also be stolen through malware installed on a user's device.

## How users can protect against such attacks

If a potentially dangerous browser extension must be installed to get one’s job done, we recommend installing it in a separate browser (or browser profile) from which the user doesn’t log in to important accounts. For example, one could download the extension onto their Firefox browser, then only use their Google Chrome browser to open important accounts, such as email or bank accounts. This mitigates the risk: a browser extension only has access to browsing data, including session cookies, of the browser on which it is installed.

## How platforms mitigate against such attacks

On most platforms, making important changes (such as changing the password) requires re-authentication and thus cannot be done through a simple session hijack. That’s why you might be asked to re-enter your password or 2FA code when modifying some settings (such as changing your password or adding new devices) on your email, social media, or other accounts.

**Additional Background**: Platforms mitigate against such attacks by asking someone to re-authenticate in case it detects suspicious behavior (for example, if a session cookie is suddenly used in a very different location or a different browser). However, adversaries are known to use proxy networks to make the continued sessions seem natural, and thus may continue to be effective in bypassing these mitigations. Platforms should also follow best practices by utilizing security attributes when setting cookies, such as Secure, HttpOnly, and SameSite, which respectively prohibit or control non-HTTPS connection transmission, client-side JavaScript access to cookies, and Cookie requests from other domains. Other protocol and procedure improvements such as binding a cookie to browser or device attributes, and short session validity periods tied with the use of refresh tokens will also limit the effectiveness of session hijacking attacks.

## Conclusion

Protecting your accounts is a shared responsibility between you (i.e. being careful in your online activities) and the configurations made by the platform provider. Practically speaking, the best steps YOU can take to avoid session hijacking attacks are: only using highly-vetted browsers and trusted extensions; and protecting your device from malware.

\
\
\

*This infosheet was developed in December 2024 for Internews partners and fellows delivering digital security training activities. You are welcome to adapt, edit, or translate this sheet based on your training needs.*

The above content has been released under the [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license

