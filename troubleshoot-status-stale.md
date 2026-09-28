---

copyright:
  years: 2026
lastupdated: "2026-09-28"

keywords: ibm cloud migration status, migration status not updating, stale migration status, migration progress, migration dashboard

subcollection: migration

content-type: troubleshoot

---

{{site.data.keyword.attribute-definition-list}}

# Why is my migration status not updating?
{: #troubleshoot-status-stale}
{: troubleshoot}

Resolve issues with {{site.data.keyword.cloud_notm}} migration status not updating. Learn how to refresh your {{site.data.keyword.mh_short}} dashboard, verify migration steps, and contact support if progress is not reflected.
{: shortdesc}

After completing one or more migration steps, the status in {{site.data.keyword.mh_short}} still shows the previous state and does not update to reflect your progress.
{: tsSymptoms}

{{site.data.keyword.mh_short}} tracks migration progress through Resource Controller attributes. Status updates depend on the service reporting the change back to Resource Controller. Delays can occur if the service has not yet propagated the status change, or if there is a temporary issue with the status reporting pipeline.
{: tsCauses}

Try the following steps:

1. Refresh the {{site.data.keyword.mh_short}} dashboard and wait a few minutes before checking again. Status updates may take several minutes to propagate.
1. Confirm that the migration step you completed was fully finalized in the target service. Navigate to the target service to verify the resource exists and is active.
1. If the status remains stale after 30 minutes, refer [Migration help](/docs/migration?topic=migration-help) and reference the migration topic ID shown in {{site.data.keyword.mh_short}}.
{: tsResolve}
