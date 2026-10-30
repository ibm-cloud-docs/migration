---
copyright:
  years: 2026

lastupdated: "2026-10-30"

keywords: migration topics, migration options, classic to vpc, clusters migration, data services migration, hpcs to key protect, key protect dedicated, servers migration, migration hub

subcollection: migration

---

{{site.data.keyword.attribute-definition-list}}

# Understanding the migration topics in Migration Hub
{: #understanding-migration-topics}

Explore migration topics and assets in IBM Cloud {{site.data.keyword.mh_short}} to transition your resources to modern infrastructure and services.
{: shortdesc}

{{site.data.keyword.mh_short}} identifies the resources in your account that require action, helps you plan your migration path, and guides you through each step.

The {{site.data.keyword.mh_short}} page includes the following sections:

- **Migration topics**: Explore and choose from multiple migration options.
- **Assets**: View the resources in your account that are eligible for migration.
- **Benefits of IBM Virtual Private Cloud**: Learn why to move to VPC.
- **Learning center**: Access insights, documentation, and help resources.

## Migration topics
{: #migration-options}

This section displays each migration category with its migration type and a brief description. {{site.data.keyword.mh_short}} provides a guided migration process across the following key infrastructure and service categories:

| Category | Migration topic | Description | Additional information |
| -------- | --------------- | ----------- | ---------- |
| Clusters | Classic to VPC | Move container workloads from classic infrastructure to VPC to improve scalability, security, and network control. | [Migrating classic clusters to VPC clusters](/docs/containers?topic=containers-vpc-migrate-overview) |
| Compute servers | Classic to VPC | Transition virtual or bare metal servers from classic infrastructure to VPC for better performance, isolation, and cost transparency. | [Migrate to VPC](/docs/classic-to-vpc) |
| Data services | Classic to VPC | Modernize your database services on VPC infrastructure built for better performance, scale, and security. | [Overview of Gen 1 (Classic) and Gen 2 (VPC)](/docs/cloud-databases-gen2?topic=cloud-databases-gen2-overview-gen1-gen2) |
{: caption="Migration topics available in Migration Hub" caption-side="bottom"}

## Assets
{: #assets-migration}

The **Assets** section lists all the resources in your account that are eligible for migration. Use the tabs to switch between migration topics, such as **Clusters** and **Data services**. Use the **Search** field to find a specific resource.

The table includes the following columns:

| Column | Description |
| ------ | ----------- |
| Name | The name of the resource. |
| Location | The region where the resource is located, for example, Dallas (us-south). |
| Tags | The tags that are assigned to the resource, for example, `env:classic`. If a resource has more tags, a count such as **+3** is shown. |
| Migration status | The current migration state of the resource, for example, **Not started**. |
| Migrate | The **Open wizard** link, which launches the migration wizard for the resource. |
{: caption="Columns in the Assets table" caption-side="bottom"}

Column names and layout vary by migration topic, as it is customized by the service product teams.
{: note}

The **Migrate or Action** column displays either an **Open wizard** link for resources ready to migrate or an in-progress status indicator. Click **Open wizard** to launch a step-by-step migration wizard that is built and maintained by the service team responsible for that resource type. The wizard guides you through the migration process with instructions, configuration steps, and validation checks specific to your resource.

For more information about the resources table and the **Open wizard** link, see [Viewing classic resources in the IBM Cloud Migration Hub](/docs/migration?topic=migration-overview-ui).

## Next steps
{: #migration-topics-next-steps}

- [Learn more about {{site.data.keyword.mh_short}}](/docs/migration?topic=migration-about-migration-hub)
- [Review migration best practices](/docs/migration?topic=migration-best-practices)
- [Review frequently asked questions](/docs/migration?topic=migration-faq)
