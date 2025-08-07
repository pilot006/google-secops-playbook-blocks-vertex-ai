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
