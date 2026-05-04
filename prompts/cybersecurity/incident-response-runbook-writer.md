---
title: Incident Response Runbook Writer
industry: cybersecurity
tags: [incident-response, runbook, soc, playbook, security-operations]
contributor: justfathi
---

## Description
Generates a step-by-step incident response runbook for a specific threat scenario — covering detection, containment, eradication, recovery, and post-incident review with role assignments and decision trees.

## Use Case
Security operations teams, SOC analysts, and DevSecOps engineers who need documented runbooks for common incident types but lack the bandwidth to write them from scratch for every threat scenario.

## The Prompt
```
You are a senior incident response engineer writing an operational runbook for a specific threat scenario. The runbook must be executable under pressure by an on-call engineer who has never handled this exact incident type before.

Incident scenario:
- Incident type: [e.g. "Ransomware deployment", "Credential stuffing attack", "Data exfiltration via compromised API key", "Insider threat — unauthorised data access", "DDoS attack on public endpoints"]
- Affected environment: [e.g. "AWS-hosted SaaS platform", "On-premise Active Directory environment", "Kubernetes cluster in GCP"]
- Tech stack involved: [LIST KEY SYSTEMS, e.g. "EKS, RDS, S3, CloudTrail, Okta, Slack"]
- SIEM / detection tools available: [e.g. "Splunk", "Datadog", "AWS Security Hub", "None"]
- IR team size and roles: [e.g. "2-person on-call rotation: engineer + security lead", "24/7 SOC team of 10"]
- Regulatory notification requirements: [e.g. "GDPR 72-hour notification", "HIPAA breach notification", "None"]

Produce a runbook with these sections:
1. Incident overview — what this is, how bad it can get, common indicators of compromise (IOCs)
2. Detection & triage — how to confirm this is a real incident vs. false positive (checklist)
3. Severity classification matrix (P1/P2/P3 with criteria)
4. Containment steps — immediate actions to limit damage (numbered, with commands or console paths where applicable)
5. Eradication steps — remove the threat root cause
6. Recovery steps — restore to known-good state
7. Evidence collection checklist — what to preserve before containment actions
8. Communications plan — who to notify, when, and what to say (templates for internal Slack, status page, legal/compliance)
9. Post-incident review template — 5 questions to answer within 48 hours
10. Runbook owner and last-reviewed date (placeholder)

Format as a document an engineer can follow under pressure. Use numbered steps, not paragraphs.
```

## Notes
- Include real command examples if you specify the tech stack — ask the model to add AWS CLI, kubectl, or equivalent commands where relevant
- The communications plan section is often skipped in runbooks but is the highest-value section during an actual incident
- Review and test runbooks in tabletop exercises at least quarterly — untested runbooks fail under pressure
