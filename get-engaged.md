---

copyright:
  years: 2026

lastupdated: "2026-08-04"

keywords: migration hub engagement, qualify for migration, migration types, when to engage, migration eligibility

subcollection: migration-service-engagement

---

{{site.data.keyword.attribute-definition-list}}

# Get engaged with {[mh]}
{: #get-engaged}

Engage with {[mh]} as early as possible — ideally at the point you know a migration is required. The earlier your team starts, the more time is available for planning, approvals, and tooling before customers must act.
{: shortdesc}

## When to engage with {[mh]}
{: #when-to-engage}

Begin the process of opening a {[mh]} engagement issue when any of the following scenarios apply:

- You are deprecating a feature or service and customers must stop using it by a certain date.
- You are moving customers to new infrastructure — for example, from Classic to VPC — and the change cannot be made silently on their behalf.
- You are upgrading to a new version or architecture that requires customers to re-provision, reconfigure, or migrate their data.
- You are relocating resources to different regions and customers must take action to remain in service.
- You have a hard deadline by which all affected resources must be migrated, whether customer-driven or business-driven.

Your GA release into the {[mh]} should be completed before any external announcement or customer-facing communications point to those materials.

### Milestone guidance
{: #milestone-guidance}

Match your engagement timing to your migration lifecycle. The full engagement process — from initial investigation to Migration Task GA — typically takes 9–17 weeks (2–4 months). If your customer deadline is shorter than that, engage the {[mh]} team immediately so that scope and timeline can be adjusted.

The following table shows recommended actions at each milestone.

| Milestone | Recommended action |
| --------- | ------------------ |
| Decision made to deprecate or migrate | Begin the "Knowing your service" phase. Open a GitHub issue in the {[mh]} repo to register intent. |
| PMT/MMT planning underway | Include {[mh]} engagement in your plan. Identify stakeholders and draft the Migration Hub section of your deck. |
| 60–90 days before customer deadline | Materials should be GA. Trigger the IBM Cloud Notification process so customers have adequate lead time. |
| 30 days before customer deadline | All materials must be in production. Send reminder notifications. Brief the support team. |
{: caption="Recommended actions by migration milestone" caption-side="bottom"}

### Customer volume is not a prerequisite
{: #customer-volume}

{[mh]} is appropriate regardless of how many customers are affected. A migration with ten affected accounts benefits from the same consistent framework as one with ten thousand. {[mh]} scales to any size engagement.

## Types of migrations that qualify
{: #migration-types}

{[mh]} supports any situation in which customers must take action on their IBM Cloud resources because of a change driven by a service team.

### In-scope migration types
{: #in-scope-types}

The following table describes the migration types that qualify for {[mh]} support.

| Type | Description | Example |
| ---- | ----------- | ------- |
| Infrastructure upgrade | Moving resources from one infrastructure generation to another. | Classic IaaS to VPC virtual servers |
| Service deprecation | A service or service plan is being retired and customers must move to a replacement. | Legacy database plan to new plan |
| Version upgrade | A major version change that requires customer action to remain supported. | PostgreSQL 12 to PostgreSQL 16 |
| Regional relocation | Resources must move to a different or consolidated region. | Single-zone region to multi-zone region |
| Architecture modernization | Moving from one architectural pattern to another within IBM Cloud. | Monolithic service to containerized service |
| Multi-service or program migration | A broader initiative not tied to a single service that requires coordinated customer action. | Classic network program migration |
{: caption="In-scope migration types" caption-side="bottom"}

### Eligibility criteria
{: #eligibility-criteria}

A migration qualifies for {[mh]} when all of the following are true:

1. **Customer action is required.** If the migration can be completed silently by IBM with no customer-visible change, it does not need to surface in the Hub.
2. **Affected resources can be identified.** The Hub relies on a Lucene query against the Ghost API to discover resources. Your team must be able to define and validate that query.
3. **A migration path exists.** Customers must have a documented path to complete the migration — documented manual steps, scripted steps, a script they run, or a full {[mh]} wizard. {[mh]} does not support discovery-only scenarios with no available action.
4. **A responsible service team exists.** Someone must own the Migration Task configuration, maintain the overview content, and support customers through completion.

### Scenarios that don't fit neatly
{: #edge-cases}

{[mh]} is flexible. It handles multi-step migrations with dependencies, migrations requiring manual approvals, and migrations with complex eligibility rules. If your scenario is unusual, engage the team early — through the GitHub issue, Slack, or office hours — rather than trying to force-fit a pattern.

### Out-of-scope migrations
{: #out-of-scope}

The following migration types are out of scope for {[mh]}:

- **Silent platform migrations** — changes that IBM makes on behalf of customers with no required customer action.
- **Cross-cloud migrations** — moving workloads from IBM Cloud to another cloud provider.
- **Customer-initiated moves** — customers reorganizing their own resources without any service team–driven change.



