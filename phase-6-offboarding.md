---

copyright:
  years: 2026

lastupdated: "2026-08-05"

keywords: migration hub phase 6, offboarding, migration task removal, closing migration, final adoption report, migration complete, decommission migration task

subcollection: migration-service-engagement

content-type: howto

---

{{site.data.keyword.attribute-definition-list}}

# Offboarding
{: #phase-offboarding}

The final phase of the Migration Hub engagement covers the retirement of a migration task from the Migration Hub console once the migration is complete and the task is no longer needed.
{: shortdesc}

Customers who have already migrated must not continue to see a task that no longer applies to them. Clean offboarding keeps Migration Hub relevant and uncluttered. Offboarding requires close coordination with the Migration Hub platform team to ensure the removal is clean — no broken links, no orphaned resources, and no customers who are mid-migration when the task is removed.

## Key deliverables
{: #phase6-deliverables}

- Confirmation that all eligible resources have migrated or the migration deadline has passed
- Any remaining customers notified and accounted for
- Migration Hub platform team engaged for removal coordination
- Pull request submitted to remove the migration task from production
- Migration task removed from `cloud.ibm.com/migration`
- GitHub engagement issue formally closed
- Final adoption report documented and shared with leadership

## Confirming migration completion
{: #phase6-confirm-completion}

Before initiating offboarding, confirm that one of the following conditions is true:

- All eligible resources have completed the migration successfully.
- The migration deadline has passed and no further customer migrations are expected.

Check your adoption metrics against the baseline count of eligible resources. If any resources remain unmigrated, assess whether they represent an active migration in progress or abandoned attempts. Notify affected customers and give them a final window to complete before proceeding with offboarding.

Do not offboard while any customer migration is actively in progress. Verify the status of all in-progress migrations in the asset table before coordinating with the Migration Hub platform team.
{: important}

## Coordinating with the Migration Hub platform team
{: #phase6-coordination}

Contact the Migration Hub platform team through your designated escalation Slack channel to initiate offboarding. The platform team coordinates the timing and reviews the removal pull request to ensure:

- No other migration tasks have dependencies on your migration topic folder.
- No active deep links from customer notifications or external documentation point to your migration task URL.
- The removal is scheduled during a low-traffic window to minimize customer impact.

For contact details, see [Help and support](/docs/migration-service-engagement?topic=migration-service-engagement-contact).

## Submitting the removal pull request
{: #phase6-removal-pr}

Submit a pull request to remove your migration topic folder from `apps/migration-hub/migrations/<topic-id>/`. The pull request is reviewed by the Migration Hub platform team before merging.

After the pull request is merged and the build is promoted to production, the migration task is no longer visible in the Migration Hub console at `cloud.ibm.com/migration`.

## Closing the GitHub engagement issue
{: #phase6-close-issue}

After the migration task is removed from production, close your GitHub engagement issue in the Migration Hub repository. Add a final comment summarizing the migration outcome: total resources migrated, final completion rate, and the closure date.

## Delivering the final adoption report
{: #phase6-final-report}

Document the migration outcomes in a final adoption report and share it with your leadership team. The report should include:

- Total eligible resources at migration launch
- Total resources migrated and final completion percentage
- Timeline from GA to closure
- Key blockers encountered and how they were resolved
- Lessons learned for future migrations

## Exit criteria
{: #phase6-exit}

The migration task is removed from production; the GitHub engagement issue is closed; the final report is delivered. The Migration Hub service engagement is complete.
