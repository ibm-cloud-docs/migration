---

copyright:
  years: 2026

lastupdated: "2026-09-21"

keywords: ibm cloud migration dashboard, classic resources, migration status, classic to vpc, classic infrastructure, migration progress, migration hub

subcollection: migration

---

{{site.data.keyword.attribute-definition-list}}

# Viewing your classic resources dashboard in {{site.data.keyword.mh_short}}
{: #overview-ui}

The **Classic resources** page is the central IBM Cloud migration dashboard for {{site.data.keyword.mh_short}}. It shows classic infrastructure resources across clusters, data services, and other resource types, tracks how many resources have moved to VPC, and helps you plan your migration to {{site.data.keyword.vpc_short}} and modern services.
{: shortdesc}

Use the **Location**, **Group**, and **Tags** filter controls to narrow data across all sections of the dashboard.

## Key metrics
{: #overview-kpi-tiles}

You can view the total number of resources in your account, the resources that are still on classic infrastructure and pending for migration, and the resources that have already migrated to VPC.

| Metric | Description |
| ------- | ----------- |
| Total resources | The total number of resources in your account that are subject to migration. |
| Classic resources | The number of resources still on classic infrastructure. |
| VPC resources | The number of resources that have already moved to VPC. |
{: caption="Key metrics on the Classic resources page" caption-side="bottom"}

## Resources in classic infrastructure
{: #overview-classic-resources}

The chart shows the total number of resources and their current migration state. The colored segments represent four states: **Not started** (gray), **In progress** (blue), **Complete** (green), and **Errors** (red).

When no Classic resources are found for your account, the chart displays **0** and a message "No classic resources found for this account."

The **Overall migration progress** shows a progress bar with the percentage of resources that have completed migration. When no migrations have been completed, the bar displays **0% Complete**.

The **Migration readiness by resources** section provides a detailed, tabular view of individual resources and their readiness to migrate. Use the tabs to switch between resource types.

## Resources in classic infrastructure table
{: #overview-resources-table}

The resources table lists classic infrastructure resources that are eligible for migration, organized by resource type. Use the tabs to switch between resource types. 

### Plan your migration
{: #overview-plan-table}

Each row shows a resource's **Name**, **Region**, **Migration status**, **Migrate** columns. The **Migrate** column displays either an **Open wizard** link for resources ready to migrate or an in-progress status indicator. The **Open wizard** link launches out the migration wizard customized by the service teams. 
