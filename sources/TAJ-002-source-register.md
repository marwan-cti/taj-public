# Source Register — TAJ Note 002

This register supports: **TAJ Note 002 — Malwares intégrant des LLM à l’exécution**.

## Admiralty scale reminder

- **A**: reliable source
- **B**: generally reliable source
- **1**: confirmed information
- **2**: probably true information
- **3**: possibly true information

## Evidence matrix

| Source | Case | Observed fact | Evidence type | Limitation | Admiralty note | Proof strength | Impact on hypothesis |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| CERT-UA | LAMEHUG | Malware uses Qwen 2.5 via the Hugging Face API to generate system commands in real time. | Real operation | Focused on attacks targeting the Ukrainian public sector. | A2 | High | Confirms at least one concrete operational case. |
| Google Cloud Blog | PROMPTSTEAL / LAMEHUG | APT28 used malware querying an LLM in live operations. | Real operation | Vendor source with its own threat visibility. | B2 | High on the case, medium on generalization. | Validates operational use for at least one public case. |
| MITRE ATT&CK | LAMEHUG | MITRE references LAMEHUG as malware directly integrating AI into its attack workflow. | Framework / knowledge base | Synthesizes third-party reporting from CERT-UA, Google and others. | A2 | High | Legitimizes the technique as an industry-tracked malware behavior. |
| ESET | PromptSpy | Gemini is used to analyze Android UI and provide step-by-step instructions for persistence. | Prototype / PoC | Not observed in ESET telemetry at publication time. | B3 | Medium | Emerging technical signal on mobile malware. |
| SentinelOne | MalTerminal | GPT-4 is used to dynamically generate ransomware code or a reverse shell. | Prototype / research | No evidence of in-the-wild deployment or distribution. | B3 | Medium | Emerging signal for dynamic payload generation. |
| NCSC | General | AI will almost certainly make elements of cyber intrusion operations more effective and efficient. | Strategic assessment | Forward-looking assessment to 2027. | A2 | Low technical, high strategic | Supports the hypothesis of growing defender relevance. |
| Google Cloud Blog | PROMPTFLUX | Gemini is used experimentally for self-obfuscation and source-code mutation. | Experimental research | Development-stage malware with no demonstrated victim compromise capability. | B3 | Medium on capability, low on operational impact | Emerging signal for AI-assisted metamorphism. |

## Source links

- Google Cloud Threat Intelligence — [GTIG AI Threat Tracker: Advances in Threat Actor Usage of AI Tools](https://cloud.google.com/blog/topics/threat-intelligence/threat-actor-usage-of-ai-tools/)
- MITRE ATT&CK — [LAMEHUG, Software S9035](https://attack.mitre.org/software/S9035/)
- ESET — [ESET Research discovers PromptSpy](https://www.eset.com/us/about/newsroom/research/eset-research-discovers-promptspy-first-android-threat-using-genai/)
- SentinelOne — [Prompts as Code & Embedded Keys: The Hunt for LLM-Enabled Malware](https://www.sentinelone.com/labs/prompts-as-code-embedded-keys-the-hunt-for-llm-enabled-malware/)
- NCSC — [Impact of AI on cyber threat from now to 2027](https://www.ncsc.gov.uk/report/impact-ai-cyber-threat-now-2027)
- Cato Networks — [Analyzing LAMEHUG](https://www.catonetworks.com/blog/cato-ctrl-threat-research-analyzing-lamehug/)

## Notes

The CERT-UA source is treated as primary for LAMEHUG, but a direct official URL should be added if available. Until then, the public portfolio note relies on corroboration through MITRE ATT&CK, Google Cloud and Cato Networks.
