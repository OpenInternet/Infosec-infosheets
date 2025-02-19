This is a fully text-based description of the *unsuccessful phishing attack* infographic.

This infographic describes an unsuccessful phishing attack. The adversary was unable to carry out this attack because the user was using a physical security key.

The graphic looks at three levels: what the user is doing, what the phishing website is doing, and what the adversary does.

On the first step, the user accidentally visits a phishing website and enters their username and password.

The second step starts with heavily emphasized text which says **Phishing Attempt is Unsuccessful**. The phishing site enters the password into a real website, which then asks for a response from the user’s physical security key. The phishing site cannot supply the response; the attack fails. (We add a footnote here. The footnote explains that if the legitimate website allows the user to ‘authenticate another way’ (such as by providing a one-time code from an authenticator app, a backup code, or an SMS code), the adversary could still try to obtain this less secure code. This ‘downgrading attack’ is why programs like Google’s Advanced Protection Program are useful, as they eliminate phishable authentication methods.)

We explain that the phishing site will give up at this stage - but the following steps are still included to show WHY exactly the attack would fail. When we outline the next steps, we use a color palette that de-emphasizes their importance, as to highlight that they are purely hypothetical.

In step 3, we explain that, even if the phishing site asked the user for their physical security key, it would not be able to obtain the correct response from the key, since the phishing site has a different domain than the website where the key was registered

In step 4, we explain that, even if the phishing site tried to forward a response it received from the security key, that response would be invalid as it’s not tied to the correct domain. It cannot be used to access the real website.

In step 5, we explain that, even if the phishing site captured the user’sp assword, it is unable to use it to log into the real website, due to the physical security key requirement.

To conclude, in this scenario the adversary behind the phishing website has no access to the user’s account—only the user does.

We designed the layout of the two infographics—which respectively describe successful and unsuccessful phishing attacks—to be very similar to each other. That way, if they are printed out or displayed side by side, it is easy to understand at which point the phishing attack would succeed or fail.