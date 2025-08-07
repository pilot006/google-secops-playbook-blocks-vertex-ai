# Google SecOps Playbook Blocks for Gemini-Assisted Case Handling

Unofficial set of Google SecOps SOAR playbook blocks that leverage Gemini on Vertex AI to assist with alert/case handling


## AI Alert Triage
Triage an alert as True/False Positive leveraging SecOps knowledge, including: Alert details, UDM query resuts, GTI enrichment, and similar case history. Details on the design of this playbook are available in [this Medium post](https://medium.com/@cloudymike/implementing-custom-ai-investigators-in-vertex-ai-for-google-secops-51fb0baaf458).


**Integrations Required**
| Parameter  | Description |
| ------------- | ------------- |
| [Vertex AI](https://cloud.google.com/chronicle/docs/soar/marketplace-integrations/vertex-ai) | Generate UDM query based on event, Triage alert with knowledge |
| [Google Chronicle](https://cloud.google.com/chronicle/docs/soar/marketplace-integrations/google-chronicle) | Run UDM query |
| [Google Threat Intelligence](https://cloud.google.com/chronicle/docs/soar/marketplace-integrations/google-threat-intelligence) | Enrich entities with GTI intel |
| [Tools](https://cloud.google.com/chronicle/docs/soar/marketplace/power-ups/tools) | Get original alert JSON |
| [Siemplify](https://cloud.google.com/chronicle/docs/soar/marketplace-integrations/siemplify) | Get similar cases|

**HTML Widget Source Code**

Source code available [here](https://raw.githubusercontent.com/pilot006/google-secops-playbook-blocks-vertex-ai/refs/heads/main/html_widget_code/ai-triage.html). Paste this in to your HTML widget code section to render results as a widget in an alert view.

**Example Output**

![AI Triage](/examples/ai-alert-triage.png?raw=true)
