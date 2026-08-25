---

copyright:
  years: 2026
lastupdated: "2026-08-25"

keywords: ibm cloud migration best practices, cloud service upgrade, migration planning, migration strategy, service deprecation, workload migration

subcollection: migration

---

{{site.data.keyword.attribute-definition-list}}

# Preparing for {{site.data.keyword.cloud_notm}} service upgrades: {{site.data.keyword.mh_short}} best practices
{: #best-practices}

Learn how to prepare for {{site.data.keyword.cloud_notm}} service upgrades and deprecations, ensuring uninterrupted workloads and smooth migrations with these best practices.
{: shortdesc}

## Planning your migration
{: #planning-migration}

Assess your current environment and understand what the migration involves before you begin.

1. Document your resources, dependencies, and configurations.
1. Use {{site.data.keyword.mh_short}}'s discovery features to identify which resources are eligible for migration.
1. Compare features between source and target products, and note any gaps that need alternative solutions.
1. Estimate costs and plan for potential downtime.
1. Set a realistic timeline based on the complexity of your migration.

## Executing your migration
{: #executing-migration}

Follow these steps to run your migration with minimal risk and disruption.

1. Launch the migration wizard in {{site.data.keyword.mh_short}} for your source product and follow the guided steps.
1. Schedule migrations during maintenance windows or low-traffic periods.
1. Test in a non-production environment before migrating production workloads.
1. Use blue-green deployments where possible so you can roll back quickly if needed.
1. Keep source and target environments running in parallel until cutover is complete.
1. Track progress using {{site.data.keyword.mh_short}}'s real-time status tracking.

## Verifying success
{: #verifying-success}

After the migration completes, confirm that your resources and workloads are functioning as expected.

1. Verify that all resources migrated to the target product.
1. Test for expected behavior and data integrity.
1. Compare performance metrics against your pre-migration baseline.
1. Review security settings and access controls in the new environment.

## Post-migration optimization
{: #post-migration}

Take advantage of your new environment to improve performance, reduce costs, and document what you learned.

1. Explore features in the target product that weren't available before.
1. Optimize configurations for the new product's architecture.
1. Set up monitoring and alerting based on pre-migration performance baselines.
1. Adjust resource allocations based on actual usage and review costs regularly.
1. Document key migration decisions, configurations, and any custom solutions.
1. Share your feedback to improve future migrations.

## Common migration challenges
{: #common-challenges}

Review these known challenges and how to address them before you start your migration.

- **Feature parity gaps**: Some features in your source product may not have direct equivalents in the target. Review {{site.data.keyword.mh_short}}'s feature comparison documentation and plan alternative implementations.

- **Data migration complexity**: Large datasets or complex data structures may require specialized tools. Use {{site.data.keyword.mh_short}}'s recommended tooling for your specific data migration needs.

- **Configuration differences**: Product configurations can differ significantly between source and target. Document all configurations and use {{site.data.keyword.mh_short}}'s guidance to map them appropriately.

- **Dependency management**: Complex service dependencies can complicate migration order. Map all dependencies before you start and plan the sequence accordingly.


## Next steps
{: #next-steps}

- [Review frequently asked questions](/docs/migration?topic=migration-faq)
- [Troubleshoot common migration issues](/docs/migration?group=troubleshooting)
- [Get help with your migration](/docs/migration?topic=migration-help)
