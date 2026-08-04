---

copyright:
  years: 2026

lastupdated: "2026-08-04"

keywords: migration hub phase 5, ongoing operations, migration support, adoption tracking, migration blockers, migration metrics, reminder notifications, migration progress reporting

subcollection: migration-service-engagement

content-type: howto

---

{{site.data.keyword.attribute-definition-list}}

# Ongoing operations
{: #phase-ongoing-operations}

The fifth phase of the {[mh]} engagement begins when your migration task goes live in production and continues until the migration is complete. The focus shifts from building to operating: actively supporting customers, monitoring adoption, identifying blockers, and refining content and tooling based on real-world feedback.
{: shortdesc}

This is not a passive phase. Customer questions need fast responses, blockers need to be found and removed, and content that is not working needs to be fixed. The migration only succeeds if customers actually complete it.

## Key activities
{: #phase5-activities}

Support customers
:   Actively respond to incoming questions and problems through support tickets, Slack, and other channels. For guidance on handling migration-related tickets and escalations, see [Supporting your customers]({[link]}-support).

Track adoption
:   Monitor how many customers have started and completed the migration. Identify customers who have not yet engaged and prioritize outreach to them.

Identify blockers
:   Analyze support patterns, {{site.data.keyword.at_short}} logs, and drop-off points to find what is stopping customers from completing the migration.

Refine content
:   Update overview pages, `config.json`, documentation, or tooling based on customer feedback. Submit pull requests to the `czero/ui` repository for any changes to the migration topic folder.

Send reminder notifications
:   Send reminder notifications per the cadence defined in your notification plan to customers who have not yet acted. For guidance, see [Informing your customers]({[link]}-inform).

Report progress
:   Share adoption metrics with leadership at agreed intervals.

## Metrics to track
{: #phase5-metrics}

Track the following metrics throughout this phase to measure progress and identify where customers are getting stuck:

| Metric | Description |
| ------ | ----------- |
| Total resources eligible for migration | Baseline count of resources that must migrate |
| Resources migrated | Count and percentage of total resources completed |
| Completion rate trend | Weekly or monthly trajectory toward full completion |
| Drop-off points | Steps in the migration flow where customers stop |
| Support ticket volume and resolution time | Indicator of friction and responsiveness |
| Time-to-complete per resource | Measure of how long the migration takes end-to-end |
{: caption="Recommended metrics for tracking migration progress" caption-side="bottom"}

## Handling blockers
{: #phase5-blockers}

When support patterns or {{site.data.keyword.at_short}} logs reveal a systemic blocker — a wizard step failing for a subset of customers, a resource discovery gap, or a translation issue — treat it as a production defect. Investigate immediately, submit a fix as a pull request, and communicate the resolution timeline to affected customers through your escalation Slack channel.

Escalate to the {[mh]} platform team for any issue that requires changes to the {[mh]} framework itself. Reach the team through your designated escalation Slack channel. For contact details, see [Help and support]({[link]}-contact).

## Exit criteria
{: #phase5-exit}

The migration deadline is reached or all eligible resources are migrated; adoption metrics are reported to leadership; your team is ready to offboard the migration task.

## Next steps
{: #phase5-next-steps}

When the migration is complete and all eligible resources have migrated (or the deadline has passed), coordinate with the {[mh]} platform team to retire the migration task. For guidance, see [Phase 6: Offboarding]({[link]}-phase-offboarding).
