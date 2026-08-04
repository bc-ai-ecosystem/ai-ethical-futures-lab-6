# 1. Detecting and Identifying AI-Generated Content

## Challenge
Generative systems produce highly realistic synthetic audio, images, video, and text. Without reliable signals, Canadians cannot easily distinguish synthetic from human-created material in news, reviews, advertising, electoral content, or personal communications. Deepfakes amplify fraud, non-consensual intimate imagery, and information-integrity risks. Over-labelling risks signal fatigue; under-labelling enables deception. Defining “AI involvement,” choosing disclosure forms, and deciding intervention points remain difficult.

## Questions
* Would it help you trust what you see online if you could tell whether content was created or modified by AI? For which types of content and in which contexts is this most important?  
* What technical or design approaches would best help Canadians identify AI-generated content (e.g., watermarks, disclaimers, provenance metadata)?  
* Who in the AI value chain should be primarily responsible for providing transparency around AI-generated content, and why? 
* Do existing market practices, technical tools, and legal frameworks make it sufficiently easy to know when content is AI-generated? If not, where are the gaps and what actions should the Government take?

## Existing Practical Solutions
- **C2PA / Content Credentials** (Coalition for Content Provenance and Authenticity, supported by Adobe Content Authenticity Initiative, Microsoft, Google, OpenAI, Meta, BBC, Intel and others): open standard embedding cryptographically signed, tamper-evident manifests that record creation tool, generative AI use, edit history, and provenance. Already implemented in Adobe tools, some camera firmware, OpenAI image outputs, and growing platform support.
- **SynthID** (Google DeepMind): invisible perceptual watermark for images, video, audio, and text that survives many transformations and is detectable by dedicated tools.
- **Platform labelling and detection**: YouTube, Meta and others apply “Made with AI” labels; Hive AI (and free Chrome extension), Illuminarty and similar multi-modal detectors classify content and often identify model families.
- Cryptographic signing of outputs by providers and research into robust multi-signal detectors (watermark + provenance + statistical).

## EU AI Act
Article 50 (applicable from 2 August 2026, with a limited grace period until 2 December 2026 for certain pre-existing systems under Article 50(2)) imposes clear, risk-based transparency duties that apply to *all* AI systems falling within its scope, not only high-risk systems.

- **Providers** of generative AI systems must ensure that outputs are marked in a machine-readable format and are detectable as artificially generated or manipulated (Article 50(2)). This is typically implemented via techniques such as C2PA Content Credentials, SynthID-style watermarks, or equivalent robust signals. The European Commission has issued guidelines and is developing a Code of Practice on Transparency of AI-generated Content to provide practical technical solutions for marking and detection.
- **Deployers** of systems that generate or manipulate image, audio or video content constituting a deepfake must disclose that the content has been artificially generated or manipulated (Article 50(4)), unless the use is authorised by law or the content is artistic/satirical and appropriate disclosures are made.
- **Deployers** of AI systems that generate or manipulate text published to inform the public on matters of public interest must disclose the artificial nature of the text (Article 50(5)), again subject to limited exceptions for human-reviewed/editorial content.

Compliant providers embed machine-readable marks at generation time and make detection tools available. Compliant deployers add human-readable labels for deepfakes and public-interest text and ensure the marks travel with the content. Fines for non-compliance can reach €15 million or 3 % of worldwide annual turnover. Exemptions exist for purely private use, artistic/satirical works, and minor edits. Major providers (OpenAI, Google, Meta, etc.) have publicly indicated compliance plans aligned with these requirements.