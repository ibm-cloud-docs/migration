---

copyright:
  years: 2026

lastupdated: "2026-09-21"

keywords: migration hub IAM, IAM permissions, resource controller access, identity access management, migration hub access, IAM roles, migration hub authentication, authorization

subcollection: migration

content-type: howto

---

{{site.data.keyword.attribute-definition-list}}

# How IAM and {{site.data.keyword.mh_short}} work together
{: #mh-iam}

{{site.data.keyword.mh_short}} uses the same [{{site.data.keyword.iamlong}} (IAM)](/docs/get-coding?topic=get-coding-iam) permissions and access controls as the Resource Controller. No additional IAM configuration is required beyond what the Resource Controller already enforces.
{: shortdesc}

Services that migrate to the Resource Controller bring their existing IAM setup with them. For the full list of required IAM roles and actions, see [IAM and the Resource Controller](/docs/get-coding?topic=get-coding-iam-rc).

## IAM permissions for {{site.data.keyword.mh_short}}
{: #mh-iam-permissions}

Any user or service ID that has the required IAM roles to interact with the Resource Controller can perform the equivalent actions in {{site.data.keyword.mh_short}}.

## Resource visibility across migration topics
{: #mh-iam-resource-visibility}

{{site.data.keyword.mh_short}} displays resources based on your IAM access, not the migration topic you belong to. If you have IAM access to resources that are managed by a different migration topic, those resources are visible to you in {{site.data.keyword.mh_short}}.

For example, if your account has IAM access to both cluster resources and data services resources, you can view both in {{site.data.keyword.mh_short}} regardless of which migration topic you are associated with.

