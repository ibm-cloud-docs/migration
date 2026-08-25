---

copyright:
  years: 2026
lastupdated: "2026-08-25"

keywords: ibm cloud migration topics missing, no migration topics, migration not showing, migration dashboard empty, IAM migration access

subcollection: migration

content-type: troubleshoot

---

{{site.data.keyword.attribute-definition-list}}

# Why don't I see any migration topics in {{site.data.keyword.mh_short}}?
{: #troubleshoot-no-topics}
{: troubleshoot}

Resolve issues with missing migration topics in IBM Cloud by checking account access, IAM roles, and notification details in {{site.data.keyword.mh_short}}.
{: shortdesc}

No migration topics appear on the {{site.data.keyword.mh_short}} dashboard, even though you received a notification about a required migration.
{: tsSymptoms}

A migration topic appears in {{site.data.keyword.mh_short}} only when all of the following conditions are true: your action is required, your affected resources are identified, a migration path is available, and a service team is responsible for the migration. If any of these conditions are not met, the topic will not display. Additionally, the topic may not be visible if you are viewing an account that does not contain the affected resources, or if you do not have the required IAM permissions to see those resources.
{: tsCauses}

Try the following steps to resolve the issue:

1. Confirm that you are logged in to the correct {{site.data.keyword.cloud_notm}} account. The affected resources must be in the account you are viewing.
1. Review the notification you received for the affected resource types and check whether those resource types exist in your account.
1. Verify that you have the appropriate IAM roles and access policies to view the resources listed in the migration notification. For more information, see [Managing access in IBM Cloud](/docs/iam?topic=iam-cloudaccess).
1. If the notification specified a start date for the migration topic, confirm that date has passed. Migration topics become visible in {{site.data.keyword.mh_short}} approximately 60–90 days before the end date.
1. If none of the above apply, contact [{{site.data.keyword.cloud_notm}} support](/docs/migration?topic=migration-help) through the {{site.data.keyword.cloud_notm}} console for assistance.
{: tsResolve}
