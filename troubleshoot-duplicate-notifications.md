---

copyright:
  years: 2026
lastupdated: "2026-08-18"

keywords: migration hub troubleshooting, migration notifications, migration already completed, duplicate notifications

subcollection: migration

content-type: troubleshoot

---

{{site.data.keyword.attribute-definition-list}}

# Why am I receiving notifications about a migration I already completed?
{: #troubleshoot-duplicate-notifications}
{: troubleshoot}

You continue to receive migration reminder notifications even though you have already completed the migration.
{: shortdesc}

IBM Cloud continues to send migration reminder notifications after you have completed the migration steps and consider the migration finished.
{: tsSymptoms}

Reminder notifications are generated based on the migration status recorded in {{site.data.keyword.mh_short}}. If the migration status in {{site.data.keyword.mh_short}} has not been updated to reflect completion — for example, because the service has not yet propagated the final status to Resource Controller{: term} — the notification system may still treat the migration as incomplete.
{: tsCauses}

Try the following steps:

1. Log in to {{site.data.keyword.mh_short}} and check the current status of the migration task. If the status still shows as incomplete or in progress, the status has not yet been updated.
1. Verify in the target service that your resources were successfully migrated and are active.
1. Allow up to 24 hours for the completion status to propagate through Resource Controller and stop triggering notifications.
1. If notifications continue after 24 hours and your migration status in {{site.data.keyword.mh_short}} is still not updated to complete, contact IBM Cloud support with your migration task ID.
{: tsResolve}
