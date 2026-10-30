---

copyright:
  years: 2026

lastupdated: "2026-10-30"

keywords: IBM Cloud migrations, migration hub, managing cloud migrations, service deprecation migration, infrastructure upgrade, cloud migration eligibility

subcollection: migration

---

{{site.data.keyword.attribute-definition-list}}

# Manage IBM Cloud migrations with Migration Hub
{: #get-engaged}

Learn how to manage IBM Cloud migrations with {{site.data.keyword.mh_short}}, the centralized platform for service deprecations and infrastructure upgrades, and IBM-initiated changes that require action on your resources.
{: shortdesc}

## Migration scenarios
{: #when-to-migrate}

{{site.data.keyword.mh_short}} applies to you when any of the following situations affect your {{site.data.keyword.cloud_notm}} account:

- Your resources are being moved to new infrastructure, for example, from Classic Infrastructure to VPC, and you must take action to complete the move.
- A major version or architecture change requires you to re-provision, reconfigure, or migrate your data.
- Resources in your account must relocate to a different region to remain in service.
- A service or feature you use is being deprecated and must be replaced by a specified deadline. Some migrations have fixed end dates, requiring affected resources to be migrated before the deadline.

You will receive notifications from {{site.data.keyword.cloud_notm}} with details about your specific situation and the actions required.

## Timeline and end dates
{: #migration-timeline}

When your migration has a published end date, {{site.data.keyword.cloud_notm}} notifies you at least 60–90 days before the end date so you have time to plan and act. The following table describes each stage of the process.

| Stage | What happens |
| ----- | ------------ |
| Migration announcement | You receive an {{site.data.keyword.cloud_notm}} notification with details about the change, the target end date (if applicable), and a link to the relevant Migration Task in {{site.data.keyword.mh_short}}. |
| End of Marketing (EoM) | Migration materials and guidance are available in {{site.data.keyword.mh_short}} 60–90 days before the end date. You can begin reviewing steps and planning your migration. Reminder notifications are sent as the end date approaches. |
| End of Support (EoS) | All affected resources must be migrated. Resources that are not migrated may be deactivated or removed. |
{: caption="Migration stages and what to expect" caption-side="bottom"}

Start the migration as early as possible. The earlier you begin, the more time you have to plan, test, and resolve any issues.
{: tip}

## Types of migrations
{: #migration-types}

{{site.data.keyword.mh_short}} supports any situation in which you must take action on your {{site.data.keyword.cloud_notm}} resources because of a service team–driven change.

### In-scope migration types
{: #in-scope-types}

The following table describes the migration types that {{site.data.keyword.mh_short}} supports.

| Type | Description | Example |
| ---- | ----------- | ------- |
| Infrastructure upgrade | Moving resources from one infrastructure generation to another. | Classic IaaS to VPC virtual servers |
| Service deprecation | A service or plan is being retired and you must move to a replacement. | Legacy database plan to new plan |
| Version upgrade | A major version change that requires action to remain supported. | PostgreSQL 12 to PostgreSQL 16 |
| Regional relocation | Resources must move to a different or consolidated region. | Single-zone region to multi-zone region |
| Architecture modernization | Moving from one architectural pattern to another within {{site.data.keyword.cloud_notm}}. | Monolithic service to containerized service |
| Multi-service or program migration | A broader initiative involving multiple services that requires coordinated action. | Classic network program migration |
{: caption="Migration types supported by {{site.data.keyword.mh_short}}" caption-side="bottom"}


### Migrations not supported by {{site.data.keyword.mh_short}}
{: #out-of-scope}

The following situations are outside the scope of {{site.data.keyword.mh_short}}:

- **Silent platform migrations:** changes that IBM makes on your behalf with no required action from you.
- **Cross-cloud migrations:** moving workloads from {{site.data.keyword.cloud_notm}} to another cloud provider.
- **Self-initiated moves:** reorganizing your own resources when no service team-driven change is involved.

## Get help
{: #migration-help}

If you have questions about a specific migration or need assistance, the following options are available:

- See [Migration help](/docs/migration?topic=migration-help) for any assistance.
- Review the notifications and documentation linked in the migration communication you received.
