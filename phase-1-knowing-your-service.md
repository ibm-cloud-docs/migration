---

copyright:
  years: 2026

lastupdated: "2026-08-05"

keywords: migration hub phase 1, knowing your service, migration planning, service engagement registration, migration stakeholders, Aha engagement, IBM Cloud Service Framework, migration timeline, migration scope

subcollection: migration-service-engagement

content-type: howto

---

{{site.data.keyword.attribute-definition-list}}

# Knowing your service
{: #phase-knowing-your-service}

The first phase of the Migration Hub engagement covers everything your service team must do before building anything. The goal is to understand the Migration Hub framework, define your migration scenario, identify the right people, establish a timeline, and decide how customers are engaged throughout the process.
{: shortdesc}

Start this phase at least three to six months before your migration task is planned to go live. Creating migration materials, reaching alignment across teams, and completing required reviews takes variable amounts of time.

The phase concludes with formal registration of intent — a GitHub issue filed with the Migration Hub team that creates a tracking record and initiates collaboration. By the end of this phase, your team is aligned, documented, and ready to build.

## Key deliverables
{: #phase1-deliverables}

- Migration type, scope, and timeline defined
- Customer engagement strategy decided — who gets notified, how, and when
- Process and tooling approach determined (wizard, docs, manual steps, or combination)
- Support process planned for customers who open help tickets
- Service identity documented (service name, PID, and short and long forms)
- Key stakeholders identified across PM, DevOps, Architecture, Design, and leadership
- PMT/MMT approval milestones scheduled
- GitHub issue submitted by using the Migration Hub **Service Onboarding Request** template

## Timeline guidance
{: #phase1-timeline}

Plan your migration at least six months before your target GA date. Use the following as a guide:

| Milestone | Recommended timing before GA |
| --------- | ----------------------------- |
| Submit service engagement intake form | 6+ months |
| Complete phase 1: Knowing your service | 5–6 months |
| Begin phase 2: Experimental staging | 4–5 months |
| Phase 3: Beta | 2–3 months |
| Phase 4: GA delivery | 0 months |
{: caption="Recommended phase timeline relative to GA" caption-side="bottom"}

## Submitting the business GitHub issue
{: #phase1-github-issue}

The product manager for the migrating service must create a **Migration Hub - Service Onboarding Request** in the [Migration Hub repository by using the provided issue template. This issue captures the high-level business context for the migration — why it is happening, what the customer impact is, and what success looks like — before any technical build work begins.

After approval, the Migration Hub team uses this issue to track your engagement and route it to the right reviewers. You can update the issue as details evolve.


## Reviewing the IBM Cloud Service Framework
{: #phase1-service-framework}

Review the [IBM Cloud Service Framework](/docs/service-framework){: external} before building anything. The Service Framework defines the standards, requirements, and processes that all IBM Cloud services must meet. Understanding where your service stands against those requirements is essential context for your migration integration.

Pay particular attention to the sections on service [lifecycle](/docs/service-framework?topic=service-framework-lifecycle){: external}, [deprecation](/docs/service-framework?topic=service-framework-deprecation-offeringplanfeature-requirements-for-end-of-support-eos){: external}, and customer communication standards, as these directly intersect with Migration Hub engagement requirements.

## Exit criteria
{: #phase1-exit}

Before proceeding to phase 2, the Migration Hub team must review and approve your readiness. The reviewer confirms the following:

- Your business GitHub issue is submitted and captures sufficient context.
- Your Aha! Epics are created and visible in the tracking view.
- Your team has reviewed the Service Framework and the full engagement expectations.
- No gaps remain that require changes before approval.

The Migration Hub team reaches out to schedule this review after your GitHub issue is submitted. After approval, your initial liaison is assigned and both teams are aligned on scope, timeline, and customer engagement approach.

## Next steps
{: #phase1-next-steps}

After your GitHub issue is approved, request CZero GitHub access through AccessHub and begin [Moving to staging](/docs/migration-service-engagement?topic=migration-service-engagement-phase-experimental-staging) phase.
