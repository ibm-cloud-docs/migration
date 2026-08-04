---

copyright:
  years: 2026

lastupdated: "2026-08-04"

keywords: migration hub phase 4, GA delivery, production deployment, customer notification, IBM Cloud notification process, migration task live, production pull request, rollback plan, support runbook

subcollection: migration-service-engagement

content-type: howto

---

{{site.data.keyword.attribute-definition-list}}

# GA delivery and customer engagement
{: #phase-ga-delivery}

The fourth phase of the {[mh]} engagement covers the final production deployment of your migration task and the execution of your customer notification strategy.
{: shortdesc}

After the production pull request is merged, affected customers can discover and act on the migration directly from the {{site.data.keyword.cloud_notm}} console. Notifications target only customers with affected resources — not your entire customer base. A tiered cadence is recommended: an initial notification well ahead of any deadline, followed by reminders as the deadline approaches.

## Key deliverables
{: #phase4-deliverables}

- Final materials reviewed and cleared for production
- Monitoring and alerting configured for the migration process and tooling
- Support team briefed; runbook created
- Rollback plan documented
- Production pull request submitted, reviewed, and merged by the {[mh]} platform team
- Migration task live at `cloud.ibm.com/migration`
- Initial customer notification sent by using the IBM Cloud Notification process
- Reminder notification cadence scheduled per plan

## Preparing for production
{: #phase4-production-prep}

Before submitting the production pull request, confirm that every item in the production sign-off criteria is met. For the full list, see [Production sign-off criteria]({[link]}-sign-off-process).

Brief your support team before the migration task goes live. Provide them with a runbook that covers:

- How to identify migration-related support tickets
- Common customer questions and their answers
- Escalation paths for issues your support team cannot resolve
- The service team's {[mh]} escalation Slack channel

Document a rollback plan before the production pull request is submitted. The plan must define the conditions under which the migration task is removed from production and the steps to do so.

## Submitting the production pull request
{: #phase4-production-pr}

The production pull request is reviewed and merged by the {[mh]} platform team — not by the service team. Coordinate with the {[mh]} team on timing before submitting.

In the pull request description, confirm:

- All phase 3 approvals are documented and linked.
- Monitoring and alerting are in place.
- The support team runbook is complete.
- The rollback plan is documented.

The pull request is processed by `CODEOWNERS` and routed to `@czero/migration-hub-approver` automatically. Do not merge without {[mh]} platform team sign-off.
{: important}

## Sending the initial customer notification
{: #phase4-notification}

Send the initial customer notification after the migration task is live in production. Target only customers with eligible resources. The notification must give customers enough lead time to plan and complete the migration before any deadline.

Your GA materials must be live before any external announcement or customer-facing communication points to them. If your customer deadline is 60 to 90 days out, the migration task must already be in production when notifications are sent.
{: important}

For full guidance on notification content, timing requirements, and the IBM Cloud Notification process, see [Informing your customers]({[link]}-inform).

## Exit criteria
{: #phase4-exit}

The migration task is live in production; the initial customer notification is sent; the migration process is handling real customer traffic with no critical errors.

## Next steps
{: #phase4-next-steps}

With the migration task live, your team transitions to active monitoring and customer support. For guidance on what is required during this phase, see [Phase 5: Ongoing operations]({[link]}-phase-ongoing-operations).
