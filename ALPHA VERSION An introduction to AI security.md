# An introduction to AI security

====
**This document is an alpha version. It is not yet ready for production or to be shared with at-risk individuals. If you see something we could improve, please let us know or submit a pull request**
====

### Distinguishing between on-device and cloud-based AI

When an AI system processes your data, for example to answer a query or transcribe some audio, it could do so either on your device or in a cloud. This is a bit like word processing: you could either use an application that just saves to your desktop, or you could use a cloud-based one. Some translation software also runs solely on-device (such as [Firefox’s translate feature](https://www.firefox.com/en-US/features/translate/)), while others rely on the cloud for such processing.

On-device AIs do all of the processing on your mobile or desktop device, and typically do not send queries back to the provider. If an AI-driven app can work offline, it’s probably only using on-device capabilities. On-device AIs offer the best privacy guarantees, though they could still reveal logs or other details if someone, such as an abusive partner or security officer conducting a search, looks through the device.

Cloud-based AIs, on the other hand, send data back to be processed on another company’s servers. This data will then be processed, stored, and shared in accordance with that company’s privacy policy–that’s why it’s important to read and regularly review those policies. Cloud-based AIs are often faster and more capable than on-device AIs, since they can rely on more data and computing power.

Some newsrooms, especially bigger ones, might be able to roll out their own servers and private clouds which run AI applications. Those could offer better performance and computing power than traditional on-device AIs without sending potentially sensitive data to other organizations.

Finally, some manufacturers are now building hybrid AI systems. They might rely on on-device capabilities for some tasks and cloud capabilities for other tasks. A well-designed hybrid AI should warn the user prior to uploading any data to the cloud.

The AI landscape remains new. Tools, capabilities, and privacy guarantees are constantly changing. As such, it’s important to regularly check back and see what processing happens on-device, what happens in the cloud, and what the cloud provider’s privacy promises are.

### Understanding how the AI keeps logs and whether it reuses them for training data

Some AI tools and chatbots will keep conversation logs, which could be stored by the organization managing or providing the AI and sometimes be read by human reviewers. It’s important to read your AI provider’s policy to understand how logs are managed, if they are ever read by humans, and if they are ever used for training data.

For examples of AI privacy and data access policies, check out those of [Google Workspace Gemini](https://support.google.com/a/answer/15706919?) or of [Microsoft 365 Copilot](https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-privacy). When reading those policies, make sure to check which tier or version of the software you are using. Many providers will offer a separate enterprise or business tier which offers additional protections, for example assuring that your logs cannot be accessed outside of the organization. Free tiers might not have all of those protections, and could potentially lead to others accessing your chat logs or histories. This will depend on which product you are using; make sure to carefully check its version and read the relevant documentation.

If you have AI chatbot conversations, and are using an enterprise or business tier of the AI software, it’s usually good to approach this with the same security mindset as documents stored on a cloud-based platform such as Google Docs or O365. You can use it for somewhat sensitive work and research but never use it for confidential information such as source names, or for cases in which the AI provider (or the country they are based in) is explicitly part of your threat model.

We strongly recommend that newsrooms use a single AI provider (or, if that’s not possible, as few providers as possible) and that they require all journalists to use that provider for work-related matters. First of all, it takes a bit of effort to keep track of different providers’ security settings and configurations and ensure that they do not keep, share, or publish logs. The fewer there are, the easier the task becomes. Secondly, work-issued AI providers will be more likely to use business or enterprise tiers and have better security guarantees. A newsroom’s system administrator might also configure your work-issued AI systems to align with privacy, security, and jurisdictional needs.

### Chat memory and history

Many AI systems offer the possibility of saving chat histories, including prompts and replies. This could be helpful, but might also expose additional information if anyone ever received access to the account or if it was shared between several people. Browse through the features of the chatbot(s) you’re using and learn how to enable, disable, and delete history.

### Hallucinations and AI poisoning

AIs frequently *hallucinate*: they can make up facts, incorrectly summarize websites, or reference non-existing resources. Always check their output to make sure it’s accurate. There are no easy rules for verifying AI outputs, though we recommend thoroughly reading through any references that a chatbot cites and making sure that they support its arguments.

Disinformation actors can also [generate large amounts of disinformation content](https://www.atlanticcouncil.org/blogs/new-atlanticist/exposing-pravda-how-pro-kremlin-forces-are-poisoning-ai-models-and-rewriting-wikipedia/) in the hope that it is picked up and quoted by chatbots and other AI systems (this practice is often called AI poisoning). Such attacks are likely to increase in frequency, which makes it even more important that we take steps to critically read and verify any AI outputs.  
