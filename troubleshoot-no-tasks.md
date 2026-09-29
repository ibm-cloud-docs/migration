---

copyright:
  years: 2026
lastupdated: "2026-09-29"

keywords: ibm cloud migration topics missing, no migration topics, migration not showing, migration dashboard empty

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

Migration topics are visible to all users who have access to {{site.data.keyword.mh_short}}. Topic visibility is not controlled by IAM roles. In most cases, all fully onboarded migration topics are visible by default. A topic might not appear if it has not yet completed the onboarding process and has not been enabled for your account.
{: tsCauses}

Try the following steps to resolve the issue:

1. Confirm that you are logged in to the correct {{site.data.keyword.cloud_notm}} account.
1. If the notification specified a start date for the migration topic, confirm that date has passed. Migration topics become visible in {{site.data.keyword.mh_short}} approximately 60–90 days before the end date.
1. If the topic is still not visible, refer the [Migration help](/docs/migration?topic=migration-help) to request that the topic be enabled for your account.
{: tsResolve}
