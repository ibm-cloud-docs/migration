---

copyright:
  years: 2026

lastupdated: "2026-08-18"

keywords: migration hub glossary, definitions, migration terms, lucene query, migration wizard, Resource Controller, service team, migration topic, IAM, blue-green deployment, Classic Infrastructure, VPC

subcollection: migration-service-engagement

---

{{site.data.keyword.attribute-definition-list}}

# Glossary
{: #glossary}

The following terms are used in {{site.data.keyword.mh_short}} documentation.
{: shortdesc}

## B
{: #glossary-b}

Blue-green deployment
:   A release strategy in which two identical environments — blue (current) and green (new) — run in parallel. Traffic is switched to the green environment after the migration is validated, and the blue environment is kept running as a fallback. {{site.data.keyword.mh_short}} recommends this strategy where possible so that you can roll back quickly if an issue is discovered after cutover.

## C
{: #glossary-c}

Classic Infrastructure
:   The original IBM Cloud infrastructure generation, based on SoftLayer, that includes classic virtual servers, bare metal servers, and classic networking. Many {{site.data.keyword.mh_short}} migration tasks guide customers from Classic Infrastructure to the newer VPC-based infrastructure.

## I
{: #glossary-i}

IAM (Identity and Access Management)
:   The IBM Cloud service that controls who can access resources and what actions they can perform. Appropriate IAM roles and access policies are required to view and manage resources in {{site.data.keyword.mh_short}}. If a migration task is not visible, insufficient IAM permissions are a common cause.

## L
{: #glossary-l}

Lucene query
:   A query string in Apache Lucene syntax used by {{site.data.keyword.mh_short}} to discover eligible customer resources through the IBM Cloud Global Search and Tagging API. The query is defined in the `discovery.luceneQuery` field of `config.json`. Common fields include `service_name`, `type`, `family`, and `region`. The `service_name` value must match the CRN segment exactly, not the console display name.

## M
{: #glossary-m}

Migration topic
:   A specific migration activity that appears as a task in the {{site.data.keyword.mh_short}} dashboard. A migration topic represents a single service team's migration offering — including the overview content, eligible resource list, and entry point into the migration wizard. Customers interact with migration topics to review requirements, track progress, and complete their migration.

{{site.data.keyword.mh_short}}
:   The IBM Cloud {{site.data.keyword.mh_short}} is the centralized platform for IBM Cloud service teams and customers to plan, coordinate, and execute migrations between IBM Cloud products and services. It provides a unified console experience for all migration motions, including Classic Infrastructure to VPC, deprecated service replacements, version upgrades, and regional relocations. The platform is generic and data-driven — service teams supply content through a pull request rather than modifying application code.

Migration wizard
:   Service-owned tooling that customers are deep-linked into from the {{site.data.keyword.mh_short}} asset table when they click **Migrate** on a resource. The wizard is built and hosted by the service team outside the `czero/ui` repository. Its URL is configured in `migrationExecution.wizardUrl` in `config.json`.

## R
{: #glossary-r}

Resource Controller (RC)
:   The IBM Cloud service that manages the lifecycle of service instances. Service teams write migration extension attributes (`migration.step`, `migration.percent`, and optional fields) to each resource instance through the Resource Controller. These attributes drive real-time migration status tracking in {{site.data.keyword.mh_short}}.

## S
{: #glossary-s}

Service team
:   An IBM Cloud service team that engages with {{site.data.keyword.mh_short}} to provide migration tooling, documentation, and support for customers migrating to or from their service. A service team typically includes a Product Management Lead, a DevOps Lead and team, a Development Architect, and a Design Lead. The migration is scoped to the specific service owned by that team.

## V
{: #glossary-v}

VPC (Virtual Private Cloud)
:   The current-generation IBM Cloud infrastructure that provides logically isolated networking, enhanced security, and greater scalability compared to Classic Infrastructure. VPC is the target platform for many {{site.data.keyword.mh_short}} migration tasks, including Classic Infrastructure to VPC migrations.

