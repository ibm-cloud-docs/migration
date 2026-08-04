---

copyright:
  years: 2026

lastupdated: "2026-08-04"

keywords: migration hub phase 3, beta, approvals, real-world testing, PMT approval, MMT approval, migration hub team approval, notification plan, Resource Controller, Activity Tracker, translations, config.json finalized

subcollection: migration-service-engagement

content-type: howto

---

{{site.data.keyword.attribute-definition-list}}

# Beta testing
{: #phase-beta-approvals}

The third phase of the {[mh]} engagement covers the refinement of all materials to near-GA quality and the completion of the migration process — whether that is a wizard, a tool, documentation, or a combination.
{: shortdesc}

Content at this stage must closely represent what customers experience at GA. The migration process must be testable end-to-end with real resources in the staging environment. This is the sign-off gate: by the end of this phase, every stakeholder has approved, the notification plan is locked, and your team is ready to ship.

## Key deliverables
{: #phase3-deliverables}

- Finalized `config.json` with complete configuration and refined resource discovery query
- Polished overview page with final messaging, design, and styling
- All required translations complete (English, German, Spanish, and French as a minimum)
- Migration process flow complete — docs, wizard, tooling, or a combination
- Resource Controller integration in place: `migration.state`, `migration.step`, and `migration.percent` attributes updating correctly
- {{site.data.keyword.at_short}} events emitting correctly for all lifecycle states
- PMT/MMT approval obtained and documented
- {[mh]} team approval obtained
- Beta testing complete with internal stakeholders or select customers using real resources
- Notification plan finalized: target audience, channel, and timing cadence locked

## Finalizing your configuration and translations
{: #phase3-config-translations}

Ensure that your `config.json` is complete and passes schema validation before submitting for review:

```sh
cd apps/migration-hub && pnpm schema:validate
```
{: pre}

Provide a `translation.json` for every required locale under `i18n/<locale>/translation.json`. Every `*Key` string in `config.json` must have a matching entry in each translation file. Missing locale files fall back to the raw key string at runtime — not the English value.
{: important}

For the full list of required fields and translation requirements, see [Building your service for migration]({[link]}-build).

## Completing Resource Controller and Activity Tracker integration
{: #phase3-backend}

Your service broker must be writing the `migration.state`, `migration.step`, and `migration.percent` extension attributes to each resource instance. These attributes drive real-time progress tracking in the {[mh]} asset table.

Your service must also emit {{site.data.keyword.at_short}} events for the full migration lifecycle. For the required event list and payload requirements, see [Integrating your service with {[mh]}]({[link]}-integrating-service).

## Obtaining approvals
{: #phase3-approvals}

Three approvals are required before your migration task can proceed to GA:

PMT/MMT approval
:   Your Product Management Team or Migration Management Team must review and approve the migration scope, timeline, and customer communication plan. Obtain this approval and document it in your GitHub engagement issue. For guidance, see [PMT / MMT process]({[link]}-pmt-process).

{[mh]} team approval
:   The {[mh]} team reviews your materials in a structured gate review. The review checks UI completeness, accessibility, configuration correctness, and documentation readiness. For guidance, see [{[mh]} team review gates]({[link]}-review).

Production sign-off
:   The final gate that confirms all criteria are met before the production pull request is submitted. For the full criteria list, see [Production sign-off criteria]({[link]}-sign-off-process).

## Running beta testing
{: #phase3-beta-testing}

Test the migration end-to-end with real resources in the staging environment before requesting any approvals. Beta testing must involve internal stakeholders or select customers who have actual eligible resources. Verify that:

- The resource discovery query returns all expected resources and no unexpected ones.
- The migration wizard launches correctly from the **Migrate** button and pre-populates with the correct context.
- Progress tracking updates correctly in the asset table as the migration proceeds.
- The migration completes successfully and the resource status updates to reflect completion.

## Locking the notification plan
{: #phase3-notification}

Before exiting this phase, finalize your notification plan. The plan must define the target audience (customers with eligible resources), the notification channel (IBM Cloud Notification process), and the timing cadence. For guidance on customer notification requirements, see [Informing your customers]({[link]}-inform).

## Exit criteria
{: #phase3-exit}

All materials are at near-GA quality in the staging environment; the migration process is tested end-to-end with real resources; all approvals are obtained and documented; the notification plan is signed off.

## Next steps
{: #phase3-next-steps}

After all approvals are in place, submit your production pull request and begin GA delivery. For guidance on what is required, see [Phase 4: GA delivery and customer engagement]({[link]}-phase-ga-delivery).
