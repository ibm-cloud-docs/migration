---

copyright:
  years: 2026

lastupdated: "2026-09-07"

keywords: migration hub overview, migration dashboard, migration status, dependency mapping, migration readiness, migration KPIs, migration progress, classic to VPC

subcollection: migration

---

{{site.data.keyword.attribute-definition-list}}

# Using the Overview page
{: #overview-ui}

The Overview page is the central dashboard for {{site.data.keyword.mh_short}}. It shows resources in your  infrastructure, helps you plan your migration, and tracks the progress of migrations across your account.
{: shortdesc}

This page currently displays sample data. Actual assessment data will be available once service teams begin contributing KPI metrics.
{: note}

## Filtering the dashboard
{: #overview-filters}

Use the **Resource group**, **Tags**, and **Region** filter controls at the top of the page to narrow data across all sections of the dashboard.

## Key metrics
{: #overview-kpi-tiles}

Four tiles near the top of the page provide at-a-glance counts for your account.

| Metric | Description |
| ------- | ----------- |
| Total resources | The total number of Classic Infrastructure resources in your account that are subject to migration. This equals the sum of resources that are ready to migrate and resources that are blocked. |
| Popular service | The service type that represents the largest share of your total resources. Shown as a count and a percentage. |
| Ready to migrate | Resources that have no migration blockers and can be migrated now. The tile also shows how many became ready this week. |
| Blocked resources | Resources that cannot be migrated until one or more blockers are resolved. The tile also shows how many blockers were added this week. |
{: caption="Key metrics on the Overview page" caption-side="bottom"}

## Overall migration progress
{: #overview-progress}

The **Overall migration progress** section provides two complementary views of your migration status.

### Donut chart
{: #overview-donut-chart}

The donut chart shows the total number of resources and their current migration state. The center of the chart displays the total resource count. The colored segments represent four states: **Not started** (gray), **In progress** (blue), **Complete** (green), and **Errors** (red).

### Estate overview and migration status
{: #overview-estate-chart}

The stacked bar chart breaks down migration states by resource type: Network, Containers, Databases, Servers, and Others.

## Migration readiness by resources
{: #overview-readiness}

The **Migration readiness by resources** section provides a detailed, tabular view of individual resources and their readiness to migrate. Use the tabs to switch between resource types.

### Filtering and searching the table
{: #overview-readiness-filters}

Use the **Blockers**, **Dependencies**, and **Search** controls to refine the list, and **Settings** to adjust which columns are displayed. 

### Plan your migration table
{: #overview-plan-table}

Each row shows a resource's **Name**, **Migration blockers** severity (None, Critical, Medium, or Minimal), **Dependencies** count (click the count to view dependent resources), and **Migration status** — either an **Open wizard** link for resources ready to migrate or an in-progress status indicator.

## Dependency mapping
{: #overview-dependency-mapping}

The **Dependency mapping** section shows how your resources are connected. Use this view to understand the impact of migrating a specific resource and to plan migration order.

### Dependency impact view
{: #overview-dependency-impact}

The dependency graph visualizes the relationships between a selected resource and its connected services. To use the dependency impact view:

1. In the **Select a resource** dropdown, choose the Classic resource that you want to analyze.
2. Review the graph to see which services and policies are connected to the selected resource.
3. Use the **Actions** menu to take action on the selected resource or its dependencies.

If you use the migration wizard, dependencies are remapped to each service automatically during migration where possible.
{: tip}

## Exporting overview data
{: #overview-export}

Use the **Export** button at the bottom of the page to download the current Overview data. The export includes the resource list and migration status information shown in the active filters.
