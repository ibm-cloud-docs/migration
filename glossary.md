---
copyright:
  years: 2026
lastupdated: "2026-09-28"
keywords: ibm cloud migration glossary, cloud migration terms, migration definitions, migration hub glossary, blue-green deployment, IAM, resource controller, migration wizard, VPC migration, migration status, service deprecation, end date, watchlist, regional relocation
subcollection: migration
---

{{site.data.keyword.attribute-definition-list}}

# {{site.data.keyword.cloud_notm}} migration glossary: Key terms and definitions
{: #glossary}

Understand key {{site.data.keyword.cloud_notm}} migration terms and definitions, including blue-green deployment, IAM, VPC, and resource controller concepts used across {{site.data.keyword.mh_short}} documentation.
{: shortdesc}

## B
{: #glossary-b}

Blue-green deployment
:   A release strategy in which two identical environments — blue (current) and green (new) — run in parallel. Traffic is switched to the green environment after the migration is validated, and the blue environment is kept running as a fallback. {{site.data.keyword.mh_short}} recommends this strategy where possible so that you can roll back quickly if an issue is discovered after cutover.

## C
{: #glossary-c}

Classic Infrastructure
:   The original {{site.data.keyword.cloud_notm}} infrastructure generation, based on SoftLayer, that includes classic virtual servers, bare metal servers, and classic networking. Many {{site.data.keyword.mh_short}} migration tasks guide customers from Classic Infrastructure to the newer VPC-based infrastructure.

Classic resources
:   The classic infrastructure resources in your {{site.data.keyword.cloud_notm}} account that are subject to migration. Classic resources are displayed on the **Classic resources** dashboard in {{site.data.keyword.mh_short}}, where you can view their migration status and take action to migrate them to VPC.

## I
{: #glossary-i}

IAM (Identity and Access Management)
:   The {{site.data.keyword.cloud_notm}} service that controls who can access resources and what actions they can perform. Appropriate IAM roles and access policies are required to view and manage resources in {{site.data.keyword.mh_short}}. If a migration task is not visible, insufficient IAM permissions are a common cause.

## M
{: #glossary-m}

Migration readiness
:   An assessment of whether a resource is ready to be migrated. In {{site.data.keyword.mh_short}}, migration readiness is shown in the **Classic resources** dashboard as a per-resource status. A resource is considered ready when it has no blockers preventing migration and the migration wizard or process is available.

Migration status
:   The current state of a resource's migration in {{site.data.keyword.mh_short}}. Each resource in the **Classic resources** dashboard displays one of four statuses: **Not started** (migration has not begun), **In progress** (migration is underway), **Complete** (migration finished successfully), or **Errors** (an issue occurred that requires attention).

Migration topic
:   A specific migration activity that appears as a task in the {{site.data.keyword.mh_short}} dashboard. A migration topic represents a single service team's migration offering — including the overview content, eligible resource list, and entry point into the migration wizard. Customers interact with migration topics to review requirements, track progress, and complete their migration.

{{site.data.keyword.mh_short}}
:   The {{site.data.keyword.cloud_notm}} {{site.data.keyword.mh_short}} is the centralized platform for {{site.data.keyword.cloud_notm}} service teams and customers to plan, coordinate, and execute migrations between {{site.data.keyword.cloud_notm}} products and services. It provides a unified console experience for all migration topics, including Classic Infrastructure to VPC, deprecated service replacements, version upgrades, and regional relocations.

Migration wizard
:   A step-by-step guided tool built and maintained by the service team responsible for a specific resource type. The wizard is launched from the **Migrate or Action** column in the {{site.data.keyword.mh_short}} resources table and guides you through the migration process with instructions, configuration steps, and validation checks specific to your resource.

Resource Controller
:   The {{site.data.keyword.cloud_notm}} platform component that manages the lifecycle of resource instances, including provisioning, access control, and metering. {{site.data.keyword.mh_short}} inherits IAM permissions directly from the Resource Controller, so no additional IAM configuration is needed to use {{site.data.keyword.mh_short}}.

## S
{: #glossary-s}

Service deprecation
:   The retirement of an {{site.data.keyword.cloud_notm}} service, plan, or feature that requires you to move to a replacement before a specified end date. Service deprecations are one of the primary triggers for migration topics appearing in {{site.data.keyword.mh_short}}.

Service product team
:   An {{site.data.keyword.cloud_notm}} service team that engages with {{site.data.keyword.mh_short}} to provide migration tooling, documentation, and support for customers migrating to or from their service. The service team owns the migration topic, defines requirements and deadlines, and builds the migration wizard.

## W
{: #glossary-w}

Watchlist
:   A list of email addresses associated with an {{site.data.keyword.cloud_notm}} support case that receive email notifications when the case is updated. Being on the watchlist does not grant access to view the case. To view a case, the account owner must grant case view access through IAM access policies.

## T
{: #glossary-t}

Topic ID
:   A unique identifier assigned to each migration task in {{site.data.keyword.mh_short}}. The topic ID is displayed in the migration task details and is used to reference a specific migration when contacting {{site.data.keyword.cloud_notm}} support or reporting an issue. Include the topic ID when you open a support case so that the support team can locate your migration quickly.

## V
{: #glossary-v}

VPC (Virtual Private Cloud)
:   The current-generation {{site.data.keyword.cloud_notm}} infrastructure that provides logically isolated networking, enhanced security, and greater scalability compared to Classic Infrastructure. VPC is the target platform for many {{site.data.keyword.mh_short}} migration tasks, including Classic Infrastructure to VPC migrations.
