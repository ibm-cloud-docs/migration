---

copyright:
  years: 2026

lastupdated: "2026-10-27"

keywords: ibm cloud migration dashboard, classic resources, migration status, classic to vpc, classic infrastructure, migration progress, migration hub

subcollection: migration

---

{{site.data.keyword.attribute-definition-list}}

# Viewing classic resources in the IBM Cloud Migration Hub
{: #overview-ui}

Use the IBM Cloud {{site.data.keyword.mh_short}} [Classic resources dashboard](/migration/classic-resources) to monitor migration progress, view resource status, and plan your move to VPC.
{: shortdesc}

Use the **Location**, **Group**, and **Tags** filter controls to narrow data across all sections of the dashboard.
{: tip}

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

When no classic resources are found for your account, the chart displays **0** and the message **No classic resources found for this account**.

The **Overall migration progress** shows a progress bar with the percentage of resources that have completed migration. When no migrations have been completed, the bar displays **0% Complete**.

## Plan your migration
{: #plan-migration}

The resources table lists classic infrastructure resources that are eligible for migration, organized by migration topic. Use the tabs to switch between migration topics. Based on the customization, the table can include columns such as **Resource name**, **Product**, **Location**, **Status**, and **Action**. 

Column names and layout vary by migration topic, as it is customized by the service teams.
{: note}

The **Migrate or Action** column displays either an **Open wizard** link for resources ready to migrate or an in-progress status indicator. Clicking **Open wizard** launches a step-by-step migration wizard built and maintained by the service team responsible for that resource type. The wizard guides you through the migration process with instructions, configuration steps, and validation checks specific to your resource.
