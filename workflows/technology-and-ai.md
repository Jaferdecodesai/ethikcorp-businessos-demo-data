# Technology & AI — current manual workflows

> SAMPLE DATA for demo – not real Ethikcorp figures
>
> Snapshot used for Businessbot automation analysis. Time estimates are illustrative weekly hours for a 4-person team (640 hours available in Oct 2026, 512 utilised, 416 billable).

## Purpose
Design and build AI-enabled transformation and workflow agents (lead qualification, approvals, routine queries, WhatsApp and voice assistants, internal knowledge assistants), plus Games Revolution work (gamification, VR/AR, learning modules). Guiding principle from the public site: fix the process before automating it; “We don’t start with AI. We start with your business.”

## Workflow 1 — Opportunity triage and solution design (6 hours / person / week)
Sales and Consulting Delivery send briefs by chat or email. An engineer or solution lead turns each brief into a short design note (systems in scope, data sources, risks, estimate). Estimates are typed into a personal spreadsheet and pasted back into the proposal.

**Friction:** briefs arrive incomplete. The same patterns (WhatsApp service agent, approvals bot, knowledge assistant) are redesigned from scratch. Security, personal-data and outbound-calling constraints are checked late.

## Workflow 2 — Build, test and hand over (12 hours / person / week)
Build work is tracked in a mix of chat threads and a lightweight task board. Environments, prompts, evaluation cases and handover notes live in folders named by the engineer. UAT is scheduled by email with the client and Consulting Delivery.

**Friction:** there is no standard evaluation set, so quality depends on who tests. Handover to Client Success is a meeting and a document, not a running runbook. Incidents after go-live come back as WhatsApp messages to the person who built the agent.

## Workflow 3 — Internal platform and reuse (4 hours / person / week)
Useful prompts, connectors and components are copied between projects when someone remembers they exist. There is no internal catalogue of reusable agents or of what is already in production at each client.

**Friction:** reuse is accidental, which keeps delivery cost high and slows proposals.

## Time that is a candidate for automation
- A structured intake form that becomes the design note and the estimate line in the proposal.
- A reusable solution catalogue (agent type, systems, estimated effort, data-protection checks).
- Standard test packs and a go-live checklist, with the runbook handed to Client Success automatically.
- A production inventory of agents, owners and next review dates.

## Expected effect if automated (illustrative, not a commitment)
Faster, more repeatable builds should improve margin on AI-agent work (a growing service line) and let the same team take on more concurrent delivery without adding headcount. A clean handover reduces unplanned aftercare that currently steals billable hours.
