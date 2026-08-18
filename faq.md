---

copyright:
  years: 2026
lastupdated: "2026-08-18"

keywords: migration hub faq, migration questions, product migration, service migration, classic to vpc, cloud foundry migration

subcollection: migration

content-type: faq

---

{{site.data.keyword.attribute-definition-list}}

# FAQs for {{site.data.keyword.mh_short}}
{: #faq}

Frequently asked questions for {{site.data.keyword.mh_short}} include questions about supported migration types, eligibility, planning, and troubleshooting. To find all FAQs for {{site.data.keyword.cloud}}, see the [FAQ library](/docs/faqs).
{: shortdesc}

## What types of migrations does {{site.data.keyword.mh_short}} support?
{: #faq-migration-types}
{: faq}

{{site.data.keyword.mh_short}} supports any situation where you must take action on your {{site.data.keyword.cloud_notm}} resources because of a service team–driven change. Supported migration types include infrastructure upgrades (for example, Classic IaaS to VPC), service deprecations, major version upgrades, regional relocations, architecture modernization, and coordinated multi-service migrations. For a complete list with examples, see [Types of migrations](/docs/migration?topic=migration-get-engaged#migration-types).

## How do I know if my resources are eligible for migration?
{: #faq-eligible-resources}
{: faq}

A {{site.data.keyword.mh_short}} task applies to your account when all of the following conditions are true: your action is required, your affected resources are identified, a documented migration path is available, and a service team{: term} is responsible for the migration. {{site.data.keyword.mh_short}} uses a Lucene query{: term} to discover which resources in your account are affected, so you can review the scope before taking action. For more details, see [When a migration applies to your account](/docs/migration?topic=migration-get-engaged#eligibility-criteria).

## What information does {{site.data.keyword.mh_short}} provide about migrations?
{: #faq-information}
{: faq}

{{site.data.keyword.mh_short}} provides a unified experience for all migration activities within the {{site.data.keyword.cloud_notm}} ecosystem. For each migration task, you can access migration rationale, benefits, costs, timelines, and other decision-making data. The platform also provides real-time account insights, service-specific migration wizards, and self-service tooling for assessing and executing migrations.

## Can I migrate resources from external cloud providers to IBM Cloud?
{: #faq-external-migrations}
{: faq}

No. {{site.data.keyword.mh_short}} supports only IBM-initiated, service team–driven changes within the {{site.data.keyword.cloud_notm}} ecosystem. Cross-cloud migrations — moving workloads from {{site.data.keyword.cloud_notm}} to another cloud provider, or from an external provider into {{site.data.keyword.cloud_notm}} — are outside the scope of {{site.data.keyword.mh_short}}. For a full list of unsupported scenarios, see [Migrations not supported by {{site.data.keyword.mh_short}}](/docs/migration?topic=migration-get-engaged#out-of-scope).

## Will my services experience downtime during migration?
{: #faq-downtime}
{: faq}

Downtime depends on the specific migration type and your implementation approach. {{site.data.keyword.mh_short}} provides guidance on minimizing service disruption, including recommendations for blue-green deployments{: term}, gradual migration strategies, and optimal maintenance windows. Many migrations can be performed with minimal or no downtime when properly planned and executed. For more information, see [Best practices](/docs/migration?topic=migration-best-practices).

## Can I roll back a migration if something goes wrong?
{: #faq-rollback}
{: faq}

Rollback capabilities depend on the specific migration type. {{site.data.keyword.mh_short}} recommends testing migrations in non-production environments first and keeping source and target environments running in parallel until cutover is complete. Some migration wizards include rollback functionality; others may require manual steps. Always review the rollback procedures documented for your specific migration before proceeding. See [Why did my migration fail, and how do I recover?](/docs/migration?topic=migration-troubleshoot-migration-failed) for recovery guidance.

## How do I track the status of my migrations?
{: #faq-track-status}
{: faq}

{{site.data.keyword.mh_short}} provides real-time migration status tracking through Resource Controller{: term} extension attributes. Your migration progress is reflected automatically in the {{site.data.keyword.mh_short}} console as the service broker writes status updates to each resource instance. Navigate to your migration task{: term} in {{site.data.keyword.mh_short}} to view current status, detailed progress information, and any required actions.

## Do I need special permissions to use {{site.data.keyword.mh_short}}?
{: #faq-permissions}
{: faq}

You need appropriate IAM{: term} roles and access policies to view and manage your {{site.data.keyword.cloud_notm}} resources in {{site.data.keyword.mh_short}}. The specific permissions required depend on the resources you are migrating and the target products. If a migration task is not visible, verify that you are logged in to the correct account and that you have the required access. For more information, see [Managing access in IBM Cloud](/docs/account?topic=account-cloudaccess).

## How do I prepare for a migration?
{: #faq-preparation}
{: faq}

Proper preparation is essential for a successful migration. Before you start, document your resources, dependencies, and configurations. Use {{site.data.keyword.mh_short}}'s discovery features to identify eligible resources, compare features between source and target products, estimate costs, and set a realistic timeline. Follow the guidance in [Best practices](/docs/migration?topic=migration-best-practices) and test your migration in a non-production environment before migrating production workloads.

## What if I encounter issues during migration?
{: #faq-migration-issues}
{: faq}

If you encounter issues during migration, review the troubleshooting topics for common problems and resolution steps:

- [Why don't I see any migration tasks?](/docs/migration?topic=migration-troubleshoot-no-tasks)
- [Why is the migration wizard unavailable?](/docs/migration?topic=migration-troubleshoot-wizard-unavailable)
- [Why is my migration status not updating?](/docs/migration?topic=migration-troubleshoot-status-stale)
- [Why are my resources not showing as eligible?](/docs/migration?topic=migration-troubleshoot-not-eligible)
- [Why did my migration fail, and how do I recover?](/docs/migration?topic=migration-troubleshoot-migration-failed)
- [Why am I receiving notifications for a completed migration?](/docs/migration?topic=migration-troubleshoot-duplicate-notifications)

If your issue is not covered, contact IBM Cloud support through the {{site.data.keyword.cloud_notm}} console.
