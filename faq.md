---

copyright:
  years: 2026
lastupdated: "2026-07-14"

keywords: migration hub faq, migration questions, product migration, service migration, classic to vpc, cloud foundry migration

subcollection: migration-hub

content-type: faq

---

{{site.data.keyword.attribute-definition-list}}

# FAQs for Migration Hub
{: #migration-hub-faq}

Frequently asked questions for Migration Hub include questions about supported migration types, migration planning, costs, and timelines. To find all FAQs for {{site.data.keyword.cloud}}, see the [FAQ library](/docs/faqs).
{: shortdesc}

## What types of migrations does Migration Hub support?
{: #faq-migration-types}
{: faq}

Migration Hub focuses on migrations within the IBM Cloud ecosystem. This includes product-to-product migrations such as Classic Infrastructure to VPC, Cloud Foundry to Code Engine, and transitions from deprecated services to their modern replacements. The MVP release does not support migrations from external sources into IBM Cloud, though this may be added in future releases.

## How do I know if my resources are eligible for migration?
{: #faq-eligible-resources}
{: faq}

Migration Hub automatically identifies resources in your account that are eligible for migration using Lucene queries. When you access Migration Hub, you'll see an overview of eligible resources in the dashboard. You can filter resources by service type, region, or migration status to find specific resources that can be migrated.

## What information does Migration Hub provide about migrations?
{: #faq-migration-information}
{: faq}

Migration Hub provides comprehensive information for each migration opportunity, including migration rationale, benefits, estimated costs, timelines, feature parity comparisons, and potential impacts. You'll also find step-by-step guidance through service-specific migration wizards and access to specialized migration tools.

## Can I migrate resources from external cloud providers to IBM Cloud?
{: #faq-external-migrations}
{: faq}

The current MVP release of Migration Hub focuses specifically on migrations within the IBM Cloud ecosystem. Migrations from external sources (such as AWS, Azure, or Google Cloud) into IBM Cloud are not currently supported but may be valuable additions in future releases.

## How long does a typical migration take?
{: #faq-migration-duration}
{: faq}

Migration duration varies significantly based on the complexity of your environment, the type of migration, the amount of data being migrated, and your specific requirements. Migration Hub provides estimated timelines for each migration scenario. Simple migrations might complete in hours, while complex enterprise migrations could take days or weeks. Use Migration Hub's planning tools to get specific estimates for your resources.

## Will my services experience downtime during migration?
{: #faq-downtime}
{: faq}

Downtime depends on the specific migration type and your implementation approach. Migration Hub provides guidance on minimizing service disruption, including recommendations for blue-green deployments, gradual migration strategies, and optimal maintenance windows. Many migrations can be performed with minimal or zero downtime when properly planned and executed.

## What are the costs associated with migration?
{: #faq-migration-costs}
{: faq}

Migration costs vary based on the source and target products, the amount of data being migrated, and the complexity of your environment. Migration Hub displays estimated costs for each migration opportunity, including both migration execution costs and ongoing operational costs for the target product. Review these estimates carefully during your planning phase.

## Can I roll back a migration if something goes wrong?
{: #faq-rollback}
{: faq}

Rollback capabilities depend on the specific migration type and your implementation approach. Migration Hub recommends testing migrations in non-production environments first and maintaining parallel systems temporarily during production migrations. Some migration wizards support rollback functionality, while others may require manual intervention. Always review the rollback procedures for your specific migration before proceeding.

## How do I track the status of my migrations?
{: #faq-track-status}
{: faq}

Migration Hub provides real-time migration status tracking through Resource Controller attributes. Navigate to the Migration Status tab in Migration Hub to view the current status of all your migrations, see detailed progress information, and identify any required actions. Status updates are displayed automatically as your migration progresses.

## What if my source product has features not available in the target product?
{: #faq-feature-parity}
{: faq}

Migration Hub provides detailed feature parity comparisons between source and target products. If certain features aren't available in the target product, Migration Hub offers guidance on alternative implementations or workarounds. Review the feature comparison documentation before starting your migration to plan for any necessary changes to your architecture or workflows.

## Do I need special permissions to use Migration Hub?
{: #faq-permissions}
{: faq}

You need appropriate access permissions to view and manage your IBM Cloud resources. The specific permissions required depend on the resources you're migrating and the target products. Ensure you have the necessary IAM roles and access policies before starting a migration. For more information, see [Managing access in IBM Cloud](/docs/account?topic=account-cloudaccess).

## What happens to my data during migration?
{: #faq-data-migration}
{: faq}

Data migration approaches vary by service type. Migration Hub provides service-specific migration wizards that include appropriate data migration tools and guidance. Data integrity and security are maintained throughout the migration process. Always validate data completeness and integrity after migration is complete.

## Can I migrate multiple resources at once?
{: #faq-bulk-migration}
{: faq}

The ability to migrate multiple resources simultaneously depends on the specific migration type and available tooling. Some migration wizards support bulk operations, while others require individual resource migration. Migration Hub helps you identify related resources and plan migration order to handle dependencies appropriately.

## How do I prepare for a migration?
{: #faq-preparation}
{: faq}

Proper preparation is essential for successful migration. Start by documenting your current environment, identifying all dependencies, reviewing feature parity between products, and understanding costs and timelines. Use Migration Hub's planning tools and follow the best practices outlined in [Migration best practices](/docs/migration-hub?topic=migration-hub-migration-best-practices). Test your migration in non-production environments before migrating production workloads.

## What if I encounter issues during migration?
{: #faq-migration-issues}
{: faq}

If you encounter issues during migration, Migration Hub provides troubleshooting guidance and access to support resources. Review the [Troubleshooting migrations](/docs/migration-hub?topic=migration-hub-troubleshoot-xx) documentation for common issues and solutions. You can also contact IBM Cloud support for assistance with complex migration problems.

## Is Migration Hub available in all regions?
{: #faq-regional-availability}
{: faq}

Migration Hub is a centralized platform accessible from the IBM Cloud console. While Migration Hub itself is globally available, the availability of specific migration paths and target products may vary by region. Check the regional availability of your target products before planning your migration.

## How often is Migration Hub updated with new migration paths?
{: #faq-updates}
{: faq}

Migration Hub is continuously enhanced with new migration paths, improved tooling, and updated guidance. As IBM Cloud products evolve and new services are introduced, Migration Hub is updated to support relevant migration scenarios. Check the [Release notes](/docs/migration-hub?topic=migration-hub-relnotes) for the latest updates and new features.
