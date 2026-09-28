---

copyright:
  years: 2026
lastupdated: "2026-09-28"

keywords: ibm cloud migration notifications, duplicate migration notifications, migration already completed, migration reminder, migration notification troubleshooting

subcollection: migration

content-type: troubleshoot

---

{{site.data.keyword.attribute-definition-list}}

# Why am I receiving notifications about a migration I already completed?
{: #troubleshoot-duplicate-notifications}
{: troubleshoot}

Stop receiving unnecessary {{site.data.keyword.cloud_notm}} migration reminder notifications after completing the migration. Learn what causes duplicate notifications and how to resolve them.
{: shortdesc}

{{site.data.keyword.cloud_notm}} continues to send migration reminder notifications after you have completed the migration steps and consider the migration finished.
{: tsSymptoms}

Reminder notifications are generated based on the migration status recorded in {{site.data.keyword.mh_short}}. If the migration status in {{site.data.keyword.mh_short}} has not been updated to reflect completion — for example, because the service has not yet propagated the final status to Resource Controller — the notification system may still treat the migration as incomplete.
{: tsCauses}

Try the following steps:

1. Log in to {{site.data.keyword.mh_short}} and check the current status of the migration task. If the status still shows as incomplete or in progress, the status has not yet been updated.
1. Verify in the target service that your resources were successfully migrated and are active.
1. Allow up to 24 hours for the completion status to propagate through Resource Controller and stop triggering notifications.
1. If notifications continue after 24 hours and your migration status in {{site.data.keyword.mh_short}} is still not updated to complete, refer [Migration help](/docs/migration?topic=migration-help).
{: tsResolve}
