---

copyright:
  years: 2026
lastupdated: "2026-09-28"

keywords: ibm cloud migration topics missing, no migration topics, migration not showing, migration dashboard empty, IAM migration access

subcollection: migration

content-type: troubleshoot

---

{{site.data.keyword.attribute-definition-list}}

# Why don't I see any migration topics in {{site.data.keyword.mh_short}}?
{: #troubleshoot-no-topics}
{: troubleshoot}

Resolve issues with missing migration topics in {{site.data.keyword.cloud_notm}} by checking account access, IAM roles, and notification details in {{site.data.keyword.mh_short}}.
{: shortdesc}

No migration topics appear on the {{site.data.keyword.mh_short}} dashboard, even though you received a notification about a required migration.
{: tsSymptoms}

A migration topic appears in {{site.data.keyword.mh_short}} only when all of the following conditions are true: your action is required, a migration process is available, and a service team is responsible for the migration. If any of these conditions are not met, the topic will not display. 
{: tsCauses}

Try the following steps to resolve the issue:

1. Confirm that you are logged in to the correct {{site.data.keyword.cloud_notm}} account. 
1. Verify that you have the appropriate IAM roles and access policies to view the the migration topics. For more information, see [Managing access in {{site.data.keyword.cloud_notm}}](/docs/iam?topic=iam-cloudaccess).
1. If the notification specified a start date for the migration topic, confirm that date has passed. Migration topics become visible in {{site.data.keyword.mh_short}} approximately 60–90 days before the end date.
1. If none of the above apply, refer [Migration help](/docs/migration?topic=migration-help) for assistance.
{: tsResolve}
