---

copyright:
  years: 2026

lastupdated: "2026-08-10"

keywords: migration hub, customer migration, migration types, migration eligibility, migration knowledge, when to migrate

subcollection: migration

---

{{site.data.keyword.attribute-definition-list}}

# What you need to know about Migration Hub
{: #get-engaged}

Migration Hub is the centralized platform for managing your IBM Cloud migrations. If you are affected by a service deprecation, infrastructure upgrade, or any other IBM-initiated change that requires action on your resources, Migration Hub provides the tools and information to help you complete the migration.
{: shortdesc}

## When Migration Hub applies to you
{: #when-to-migrate}

You may be directed to Migration Hub when any of the following situations affect your IBM Cloud account:

- A service or feature you use is being deprecated and you must stop using it by a specific date.
- Your resources are being moved to new infrastructure — for example, from Classic to VPC — and you must take action to complete the move.
- A major version or architecture change requires you to re-provision, reconfigure, or migrate your data.
- Resources in your account must relocate to a different region to remain in service.
- A hard deadline exists by which all affected resources must be migrated.

You will receive notifications from IBM Cloud with details about your specific situation and the actions required.

## Timeline and deadlines
{: #migration-timeline}

IBM Cloud aims to give you adequate lead time before any migration deadline. The following table shows what to expect at each stage.

| Stage | What happens |
| ----- | ------------ |
| Migration announced | You receive an IBM Cloud notification with details about the change, the deadline, and a link to the relevant Migration Task in Migration Hub. |
| 60–90 days before deadline | Migration materials and guidance are available in Migration Hub. You can begin reviewing steps and planning your migration. |
| 30 days before deadline | Reminder notifications are sent. Begin completing the migration if you haven't already. |
| Deadline | All affected resources must be migrated. Resources that are not migrated may be deactivated or removed. |
{: caption="Migration stages and what to expect" caption-side="bottom"}

Start the migration as early as possible. The earlier you begin, the more time you have to plan, test, and resolve any issues before the deadline.

## Types of migrations
{: #migration-types}

Migration Hub supports any situation in which you must take action on your IBM Cloud resources because of a service team–driven change.

### In-scope migration types
{: #in-scope-types}

The following table describes the migration types that Migration Hub supports.

| Type | Description | Example |
| ---- | ----------- | ------- |
| Infrastructure upgrade | Moving resources from one infrastructure generation to another. | Classic IaaS to VPC virtual servers |
| Service deprecation | A service or plan is being retired and you must move to a replacement. | Legacy database plan to new plan |
| Version upgrade | A major version change that requires action to remain supported. | PostgreSQL 12 to PostgreSQL 16 |
| Regional relocation | Resources must move to a different or consolidated region. | Single-zone region to multi-zone region |
| Architecture modernization | Moving from one architectural pattern to another within IBM Cloud. | Monolithic service to containerized service |
| Multi-service or program migration | A broader initiative involving multiple services that requires coordinated action. | Classic network program migration |
{: caption="Migration types supported by Migration Hub" caption-side="bottom"}

### When a migration applies to your account
{: #eligibility-criteria}

A Migration Hub task applies to your account when all of the following are true:

1. **Your action is required.** If IBM can complete the migration with no customer-visible change, it will not appear in the Hub.
2. **Your affected resources are identified.** Migration Hub uses a query to discover which resources in your account are affected. You can review the scope before taking action.
3. **A migration path is available.** You will have a documented path to complete the migration — step-by-step instructions, a script to run, or a guided wizard in Migration Hub.
4. **A service team is responsible.** The team that owns the service you are migrating from maintains the migration content and is available to support you.

### Migrations not supported by Migration Hub
{: #out-of-scope}

The following situations are outside the scope of Migration Hub:

- **Silent platform migrations** — changes that IBM makes on your behalf with no required action from you.
- **Cross-cloud migrations** — moving workloads from IBM Cloud to another cloud provider.
- **Self-initiated moves** — reorganizing your own resources when no service team–driven change is involved.

## Get help
{: #migration-help}

If you have questions about a specific migration or need assistance, the following options are available:

- Review the migration overview and steps in the Migration Task within Migration Hub.
- Contact IBM Cloud support through the IBM Cloud console.
- Refer to the notifications and documentation linked in the migration communication you received.
