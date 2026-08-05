---

copyright:
  years: 2026

lastupdated: "2026-08-05"

keywords: migration hub phase 2, experimental staging, stub materials, config.json, staging branch, migration task staging, migration overview page, icon.svg, translation.json

subcollection: migration-service-engagement

content-type: howto

---

{{site.data.keyword.attribute-definition-list}}

# Moving to staging
{: #phase-experimental-staging}

The second phase of the Migration Hub engagement covers the creation and delivery of initial stub materials — a minimal but functional version of your service team's migration task deployed to the staging environment.
{: shortdesc}

The goal of this phase is to get early visual feedback, validate technical configuration, and give stakeholders something concrete to react to before investing in final content. The materials at this stage are intentionally rough: a basic configuration, a placeholder overview page, initial documentation landing locations, and early process or tooling sketches. Prioritize speed of iteration over polish.

## Key deliverables
{: #phase2-deliverables}

- `config.json` with required fields: `id`, discovery query, wizard URL, and steps
- `overview.html` with placeholder messaging and structure
- Documentation landing page locations identified and stubbed
- Service icon (`icon.svg`)
- English translation file (`i18n/en/translation.json`)
- Initial process and tooling approach represented, even if placeholder
- Pull request submitted to the Migration Hub repository targeting the stage branch
- Staging review completed; stakeholder feedback gathered and documented

## Building stub materials
{: #phase2-building}

Copy the sample template from the repository as your starting point:

```sh
cp -r apps/migration-hub/migrations/sampleservice \
      apps/migration-hub/migrations/<topic-id>
```
{: pre}

Your stub `config.json` must include the minimum required fields so the migration task is discoverable and renders in the staging environment. Use placeholder strings for copy that is not yet final. For full details on every `config.json` field, see [Building your service for migration](/docs/migration-service-engagement?topic=migration-service-engagement-build).

For your stub overview page, keep messaging simple and clearly mark placeholder content. The Migration Hub team needs to be able to see the overall structure and layout — not the final copy — to give meaningful feedback.

## Submitting the staging pull request
{: #phase2-pr}

Target the `stage` branch when submitting your pull request. The pull request description must include:

- A short description of the service being migrated and the target platform
- Confirmation that the Lucene query returns correct resources in the staging environment
- Screenshots showing the migration tile and overview page rendering in staging

For the full pull request checklist, see [Building your service for migration](/docs/migration-service-engagement?topic=migration-service-engagement-build).

## Staging review
{: #phase2-review}

After your pull request is merged to the stage branch and the migration task is visible in the staging environment, schedule a staging review with the Migration Hub team. The review covers:

- Visual rendering of the opportunity tile and overview page
- Correctness of the resource discovery query
- Navigation and routing within the migration task
- Any blockers or structural issues to resolve before beta

Gather stakeholder feedback from the review and document it. This feedback drives priorities and scope decisions for the beta phase.

## Exit criteria
{: #phase2-exit}

Stub materials are merged to the stage branch; the migration task is visible in the staging environment; stakeholder feedback is gathered and incorporated into beta planning.

## Next steps
{: #phase2-next-steps}

After the staging review is complete, begin refining your materials to near-GA quality. For guidance on what is required in the next phase, see [Phase 3: Beta, approvals, and real-world testing](/docs/migration-service-engagement?topic=migration-service-engagement-phase-beta-approvals).
