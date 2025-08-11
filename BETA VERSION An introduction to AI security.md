# An introduction to AI security

====
**This document is a beta version. It is not yet ready for production or to be shared with at-risk individuals. If you see something we could improve, please let us know or submit a pull request**
====

### Distinguishing between on-device and cloud-based AI

When an AI system processes your data, for example to answer a query or transcribe some audio, it could do so either on your device or in a cloud. This is a bit like word processing: you could use an application that just saves to your desktop, or cloud-based one.

On-device AIs do all of the processing on your mobile or desktop device, and typically do not send queries back to the provider. If an AI-driven app can work offline, it’s probably only using on-device capabilities. On-device AIs offer the best privacy guarantees, though they could still reveal logs or other details if someone, such as an abusive partner or security officer conducting a search, looks through the device. It's often possible to use an on-device LLM to process highly sensitive data, though this might require some initial set up. If this is of interest to you, reach out to a digital security trainer or IT person who could help set up such a system.

Cloud-based AIs, on the other hand, process data on a company's servers. This data will be used, stored, and shared in accordance with that company’s privacy policy–that’s why it’s important to read and regularly review those policies. Cloud-based AIs are often more capable than on-device AIs, since they can rely on more data and computing power.

Finally, some manufacturers are now building hybrid AI systems. They might rely on on-device capabilities for some tasks and cloud capabilities for other tasks. A well-designed hybrid AI should warn and ask the user for permission prior to uploading any of their data to the cloud.

The AI landscape remains new. Tools, capabilities, and privacy guarantees are constantly changing. As such, it’s important to regularly check back and see what processing happens on-device, what happens in the cloud, and what the cloud provider’s privacy promises are.

### Cloud-based AIs, logs, and some recommendations

Some cloud-based AI tools and chatbots will keep logs of conversations and data you share with them. Such logs could be stored by the AI provider, used as training data for future AI systems, and sometimes be read by human reviewers. If the organization stores, processes, or otherwise uses logs, then there's a chance that any sensitive data you type into AI tools or chatbots could leak out one day. It’s therefore important to read your AI provider’s privacy policy to understand how they manage your data.

For examples of AI privacy and data access policies, check out those of [Google Workspace Gemini](https://support.google.com/a/answer/15706919?) or of [Microsoft 365 Copilot](https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-privacy). Check which tier or version of the software you are using. Many providers will have a separate enterprise or business tier which offers additional protection, such as not using your data for AI training.
Free or basic paid tiers might not have all of those protections, which could potentially allow others to access your chat logs or histories. All depends on which provider you're using.

If you have AI chatbot conversations, and are using an enterprise or business tier of the AI software, you can often adopt the same security mindset as with documents stored on a cloud-based platform such as Google Docs or O365. You can use it for somewhat sensitive work and research but never use it for confidential information such as source names, or for cases in which the AI provider (or the country they are based in) is explicitly part of your threat model.

We strongly recommend that newsrooms use a single AI provider (or, if that’s not possible, as few providers as possible), that they subscribe to the enterprise rather than free tier, and that they require all journalists to use that provider for work-related matters.
It takes effort to keep track of different providers’ security settings and configurations, pay for professional packages, and check policies to ensure that those do not keep, share, or publish logs. The fewer there are, the easier the task becomes. A newsroom’s system administrator might also be able to configure your work-issued AI systems to align with your privacy, security, and jurisdictional needs.

### Chat memory and history

Many AI systems offer the possibility of saving chat histories, including prompts and replies. This could be helpful, but might also expose additional information if anyone ever received access to the account or if it was shared between several people. Browse through the features of the chatbot(s) you’re using and learn how to enable, disable, and delete history.

Also, if in your threat model includes potential seizure, theft, or any other unauthorized acquisition of any device that can access AI chat history, also consider deleting any chatbot history frequently, or at least every time the device can be compromised, like in risky border crossings or during field coverage in sensitive contexts.

### Hallucinations and AI poisoning

AIs frequently *hallucinate*: they can make up facts, incorrectly summarize websites, and reference non-existing resources. Always check their output to make sure it’s accurate. There are no easy rules for verifying AI outputs, though we recommend thoroughly reading through any references that a chatbot cites and making sure that they support its arguments.

Disinformation actors can also [generate large amounts of disinformation content](https://www.atlanticcouncil.org/blogs/new-atlanticist/exposing-pravda-how-pro-kremlin-forces-are-poisoning-ai-models-and-rewriting-wikipedia/) in the hope that it is picked up and quoted by chatbots and other AI systems (this practice is often called AI poisoning). Such attacks are likely to increase in frequency, which makes it even more important that we take steps to critically read and verify any AI outputs.  
