---

copyright:
  years: 2026
lastupdated: "2026-08-12"

keywords: migration best practices, migration planning, migration strategy, product migration, service migration

subcollection: migration

---

{{site.data.keyword.attribute-definition-list}}

# Best practices
{: #best-practices}

When IBM Cloud notifies you about a service upgrade or deprecation, review these best practices to understand what the change means for your environment and how to prepare. Notifications include details about timelines and required updates so that your workloads remain uninterrupted.
{: shortdesc}

## Planning your migration
{: #planning-migration}

Before you start, assess your current environment and understand what the migration involves:

1. Document all resources, dependencies, and configurations in your source product.
1. Use {{site.data.keyword.mh_short}}'s discovery features to identify which resources are eligible for migration.
1. Review feature parity between the source and target products, and identify any deprecated features that require alternative solutions.
1. Review estimated migration costs and plan for any potential downtime.
1. Set realistic timelines based on the complexity of your migration and available resources.

## Executing your migration
{: #executing-migration}

1. Access the appropriate migration wizard in {{site.data.keyword.mh_short}} for your source product and follow the step-by-step guidance.
1. Schedule migrations during maintenance windows or low-traffic periods.
1. Test in a non-production environment before migrating production workloads.
1. Use blue-green deployment strategies where possible to enable quick rollback.
1. Maintain parallel systems temporarily to ensure a smooth cutover.
1. Monitor progress through {{site.data.keyword.mh_short}}'s real-time status tracking.

After the migration completes, verify success:

1. Confirm all resources migrated correctly to the target product.
1. Test functionality to ensure expected behavior and data integrity.
1. Check performance metrics against your baseline.
1. Review security configurations and access controls in the new environment.

## Post-migration optimization
{: #post-migration}

1. Review documentation for features available in the target product that were not in the source product.
1. Optimize configurations for the new product's architecture.
1. Set up monitoring and alerting, and track performance metrics against pre-migration baselines.
1. Adjust resource allocations based on actual usage patterns and review costs regularly.
1. Document migration decisions, configurations, and any custom solutions implemented.
1. Share lessons learned to improve future migrations.

## Common migration challenges
{: #common-challenges}

- Feature parity gaps: Some features in your source product may not have direct equivalents in the target. Review {{site.data.keyword.mh_short}}'s feature comparison documentation and plan alternative implementations.

- Data migration complexity: Large datasets or complex data structures may require specialized tools. Use {{site.data.keyword.mh_short}}'s recommended tooling for your specific data migration needs.

- Configuration differences: Product configurations can differ significantly between source and target. Document all configurations and use {{site.data.keyword.mh_short}}'s guidance to map them appropriately.

- Dependency management: Complex service dependencies can complicate migration order. Map all dependencies before you start and plan the sequence accordingly.


## Next steps
{: #next-steps}

- [Review frequently asked questions](/docs/migration-?topic=migration-faqs)
- [Troubleshoot common migration issues](/docs/migration-?topic=migration-troubleshoot-xx)
- [Get help with your migration](/docs/migration-?topic=migration-contact)
