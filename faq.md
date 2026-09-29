---

copyright:
  years: 2026
lastupdated: "2026-09-29"

keywords: migration hub faq, ibm cloud migration questions, migration eligibility, migration types, classic to vpc, cloud foundry migration, migration planning, migration costs

subcollection: migration

content-type: faq

---

{{site.data.keyword.attribute-definition-list}}

# {{site.data.keyword.cloud_notm}} {{site.data.keyword.mh_short}}: Frequently asked questions
{: #faq}

Get answers to frequently asked questions about {{site.data.keyword.cloud_notm}} {{site.data.keyword.mh_short}}, including supported {{site.data.keyword.cloud_notm}} migration types, eligibility, planning, costs, and timelines.
{: shortdesc}

## What types of migrations does {{site.data.keyword.mh_short}} support?
{: #faq-migration-types}
{: faq}

{{site.data.keyword.mh_short}} focuses on migrations within the {{site.data.keyword.cloud_notm}} ecosystem. This includes product-to-product migrations such as Classic Infrastructure to VPC, Cloud Foundry to Code Engine, and transitions from deprecated services to their modern replacements. The {{site.data.keyword.mh_short}} release does not support migrations from external sources into {{site.data.keyword.cloud_notm}}, though this may be added in future releases.

## How do I know if my resources are eligible for migration?
{: #faq-eligible-resources}
{: faq}

{{site.data.keyword.mh_short}} automatically identifies resources in your account that are eligible for migration. When you access {{site.data.keyword.mh_short}}, you'll see an overview of eligible resources in the dashboard. You can filter resources by service type, region, or migration status to find specific resources that can be migrated.

## What information does {{site.data.keyword.mh_short}} provide about migrations?
{: #faq-information}
{: faq}

{{site.data.keyword.mh_short}} provides comprehensive information for each migration topic, including migration rationale, benefits, estimated costs, timelines, feature parity comparisons, and potential impacts. You'll also find step-by-step guidance through service-specific migration wizards and access to specialized migration tools.

## Can I migrate resources from external cloud providers to {{site.data.keyword.cloud_notm}}?
{: #faq-external-migrations}
{: faq}

The current release of {{site.data.keyword.mh_short}} focuses specifically on migrations within the {{site.data.keyword.cloud_notm}} ecosystem. Migrations from external sources into {{site.data.keyword.cloud_notm}} are not currently supported but may be valuable additions in future releases.

## Do all migrations operate in the same way with workflow and documentation?
{: #faq-operate-all}
{: faq}

No. Each migration topic has its own workflow, documentation, and tooling, maintained by the service team responsible for that migration. Some migrations use a guided wizard, others provide step-by-step instructions or a script to run, and timelines vary by complexity. What is consistent across all migrations is that {{site.data.keyword.mh_short}} identifies the resources that require action, provides a documented process to completion, and connects you with the responsible service team. For more information, see [What you need to know about {{site.data.keyword.mh_short}}](/docs/migration?topic=migration-get-engaged).

## How long does a typical migration take?
{: #faq-migration-duration}
{: faq}

Migration duration varies significantly based on the complexity of your environment, the type of migration, the amount of data being migrated, and your specific requirements. {{site.data.keyword.mh_short}} provides estimated timelines for each migration scenario. Simple migrations might complete in hours, while complex enterprise migrations could take days or weeks. Use {{site.data.keyword.mh_short}}'s planning tools to get specific estimates for your resources.

## Will my services experience downtime during migration?
{: #faq-downtime}
{: faq}

Downtime depends on the specific migration type and your implementation approach. {{site.data.keyword.mh_short}} provides guidance on minimizing service disruption, including recommendations for blue-green deployments, gradual migration strategies, and optimal maintenance windows. Many migrations can be performed with minimal or zero downtime when properly planned and executed.

## What are the costs associated with migration?
{: #faq-migration-costs}
{: faq}

Migration costs vary based on the source and target products, the amount of data being migrated, and the complexity of your environment. {{site.data.keyword.mh_short}} displays estimated costs for each migration topic, including both migration execution costs and ongoing operational costs for the target product. Review these estimates carefully during your planning phase.

## Can I roll back a migration if something goes wrong?
{: #faq-rollback}
{: faq}

Rollback capabilities depend on the specific migration type and your implementation approach. {{site.data.keyword.mh_short}} recommends testing migrations in non-production environments first and maintaining parallel systems temporarily during production migrations. Some migration wizards support rollback functionality, while others may require manual intervention. Always review the rollback procedures for your specific migration before proceeding.

## How do I track the status of my migrations?
{: #faq-track-status}
{: faq}

{{site.data.keyword.mh_short}} provides real-time migration status tracking through Resource Controller attributes. Navigate to the Migration Status tab in {{site.data.keyword.mh_short}} to view the current status of all your migrations, see detailed progress information, and identify any required actions. Status updates are displayed automatically as your migration progresses.

## What if my source product has features not available in the target product?
{: #faq-feature-parity}
{: faq}

{{site.data.keyword.mh_short}} provides detailed feature parity comparisons between source and target products. If certain features aren't available in the target product, {{site.data.keyword.mh_short}} offers guidance on alternative implementations or workarounds. Review the feature comparison documentation before starting your migration to plan for any necessary changes to your architecture or workflows.

## Do I need special permissions to use {{site.data.keyword.mh_short}}?
{: #faq-permissions}
{: faq}

You need appropriate access permissions to view and manage your {{site.data.keyword.cloud_notm}} resources. The specific permissions required depend on the resources you're migrating and the target products. Ensure you have the necessary IAM roles and access policies before starting a migration. For more information, see [Managing access in {{site.data.keyword.cloud_notm}}](/docs/iam?topic=iam-cloudaccess).

## What happens to my data during migration?
{: #faq-data-migration}
{: faq}

Data migration approaches vary by service type. {{site.data.keyword.mh_short}} provides service-specific migration wizards that include appropriate data migration tools and guidance. Data integrity and security are maintained throughout the migration process. Always validate data completeness and integrity after migration is complete.

## Can I migrate multiple resources at once?
{: #faq-bulk-migration}
{: faq}

The ability to migrate multiple resources simultaneously depends on the specific migration type and available tooling. Some migration wizards support bulk operations, while others require individual resource migration. {{site.data.keyword.mh_short}} helps you identify related resources and plan migration order to handle dependencies appropriately.

## How do I prepare for a migration?
{: #faq-preparation}
{: faq}

Proper preparation is essential for successful migration. Start by documenting your current environment, identifying all dependencies, reviewing feature parity between products, and understanding costs and timelines. Use {{site.data.keyword.mh_short}}'s planning tools and follow the best practices outlined in [Migration best practices](/docs/migration?topic=migration-best-practices). Test your migration in non-production environments before migrating production workloads.

## What if I encounter issues during migration?
{: #faq-migration-issues}
{: faq}

If you encounter issues during migration, {{site.data.keyword.mh_short}} provides troubleshooting guidance and access to support resources. Review the [Troubleshooting migrations](/docs/migration?group=troubleshooting) documentation for common issues and solutions. Refer [Migration Help](/docs/migration?topic=migration-help) for assistance with complex migration problems.

## Is {{site.data.keyword.mh_short}} available in all regions?
{: #faq-regional-availability}
{: faq}

{{site.data.keyword.mh_short}} is a centralized platform accessible from the {{site.data.keyword.cloud_notm}} console. While {{site.data.keyword.mh_short}} itself is globally available, the availability of specific migration topics and target products may vary by region. Check the regional availability of your target products before planning your migration.

## How often is {{site.data.keyword.mh_short}} updated with new migration topics?
{: #faq-updates}
{: faq}

{{site.data.keyword.mh_short}} is continuously enhanced with new migration topics, improved tooling, and updated guidance. As {{site.data.keyword.cloud_notm}} products evolve and new services are introduced, {{site.data.keyword.mh_short}} is updated to support relevant migration scenarios. Check the [Release notes](/docs/migration?topic=migration-relnotes) for the latest updates and new features.

## How will I know if I need to use {{site.data.keyword.mh_short}}?
{: #faq-when-to-use}
{: faq}

{{site.data.keyword.cloud_notm}} sends you a notification when a service deprecation, infrastructure upgrade, version change, or regional relocation affects your account and requires action on your resources. The notification includes details about the required change, the target end date (if applicable), and a link to the relevant migration task in {{site.data.keyword.mh_short}}. You can also access {{site.data.keyword.mh_short}} directly from the {{site.data.keyword.cloud_notm}} console at any time to check whether any migration topics apply to your account.

## What happens to my resources if I do not migrate by the end date?
{: #faq-end-date-consequences}
{: faq}

When a migration topic has a specific end date, resources that are not migrated by that date may be deactivated or removed. {{site.data.keyword.cloud_notm}} aims to provide adequate lead time — typically 60 to 90 days before the end date — and sends reminder notifications 30 days before the deadline. Start your migration as early as possible to allow time to plan, test, and resolve any issues. For a full breakdown of migration stages, see [Managing {{site.data.keyword.cloud_notm}} migrations with {{site.data.keyword.mh_short}}](/docs/migration?topic=migration-get-engaged).

## Does {{site.data.keyword.mh_short}} support migrations I initiate myself?
{: #faq-self-initiated}
{: faq}

No. {{site.data.keyword.mh_short}} is designed for IBM-initiated changes that require action on your resources, such as service deprecations, infrastructure upgrades, and regional relocations. Self-initiated reorganizations — such as moving resources between accounts or regions for your own operational reasons when no service team–driven change is involved — are outside the scope of {{site.data.keyword.mh_short}}.

## What migration topics are currently available in {{site.data.keyword.mh_short}}?
{: #faq-available-topics}
{: faq}

{{site.data.keyword.mh_short}} currently supports the following migration topics:

- **Clusters (Classic to VPC)**: Move container workloads from classic infrastructure to VPC.
- **Compute servers (Classic to VPC)**: Transition virtual or bare metal servers from classic infrastructure to VPC.
- **Data services (Classic to VPC)**: Modernize database services on VPC infrastructure.

New migration topics are added as {{site.data.keyword.cloud_notm}} services evolve. For the full list of supported migration options, see [Understanding migration topics](/docs/migration?topic=migration-understanding-migration-topics).

## What migration statuses can a resource have?
{: #faq-migration-statuses}
{: faq}

Each resource on the Classic resources dashboard can have one of four migration statuses:

- **Not started**: The resource has not begun migration.
- **In progress**: Migration is underway for the resource.
- **Complete**: The resource has successfully migrated.
- **Errors**: An issue occurred during migration that requires attention.

## What is the Open wizard link in the resources table?
{: #faq-open-wizard}
{: faq}

The **Open wizard** link appears in the **Migrate** column of the resources table when a resource is ready to migrate. Clicking it launches the migration wizard that is customized by the service team responsible for that resource type. If the resource is already being migrated, the column shows an in-progress status indicator instead.

## Do I need to configure IAM separately to use {{site.data.keyword.mh_short}}?
{: #faq-iam-configuration}
{: faq}

No additional IAM configuration is required. {{site.data.keyword.mh_short}} inherits the same IAM permissions as the Resource Controller. Any user or service ID that already has the required IAM roles to interact with the Resource Controller can perform the equivalent actions in {{site.data.keyword.mh_short}}. For details on the required roles and actions, see [How IAM and {{site.data.keyword.mh_short}} work together](/docs/migration?topic=migration-mh-iam).

## I have access to resources from a different migration topic. Will I see them in {{site.data.keyword.mh_short}}?
{: #faq-cross-topic-visibility}
{: faq}

Yes. {{site.data.keyword.mh_short}} displays resources based on your IAM access, not the migration topic you are associated with. If you have IAM permissions to view resources that belong to a different migration topic, those resources are visible to you in {{site.data.keyword.mh_short}}. Your IAM policies determine which resources you can see across all migration topics.

## I was added to a support case watchlist. Why can't I view the case?
{: #faq-watchlist-access}
{: faq}

Being on the watchlist sends you email notifications when the case is updated, but does not grant access to view the case. To follow the case link in the email notification and view the case details, the account owner must use {{site.data.keyword.cloud_notm}} Identity and Access Management (IAM) access policies to grant you case view access.

## How do I get support for a specific migration issue through {{site.data.keyword.mh_short}}?
{: #faq-get-support}
{: faq}

Open the **Migration help** popup within {{site.data.keyword.mh_short}} and browse self-help resources such as migration guides, prerequisites, best practices, and troubleshooting content. If the self-help resources do not resolve your issue, click **I still need help** to open the support case flow. The support case form is scoped to {{site.data.keyword.mh_short}} topics and pre-fills with contextual information to help route your request to the correct team.

## Who is responsible for defining migration requirements and deadlines?
{: #faq-who-owns-deadlines}
{: faq}

Each migration topic is owned by the {{site.data.keyword.cloud_notm}} service team responsible for that product change. The service team defines migration requirements, sets customer deadlines, authors the migration topic content in {{site.data.keyword.mh_short}}, and provides technical support for their specific migration. The {{site.data.keyword.mh_short}} platform team builds and maintains the {{site.data.keyword.mh_short}} experience but does not set migration deadlines or requirements for individual topics. If you have questions about the timeline or requirements for a specific migration, refer to the documentation and notifications provided by the service team for that migration.
