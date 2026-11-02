---

copyright:
  years: 2026
lastupdated: "2026-10-30"

keywords: migration hub troubleshooting, resources not eligible, migration eligibility, missing resources

subcollection: migration

content-type: troubleshoot

---

{{site.data.keyword.attribute-definition-list}}

# Why are my resources not showing as eligible for migration?
{: #troubleshoot-not-eligible}
{: troubleshoot}

You believe certain resources in your account should be included in a migration task, but they do not appear in the eligible resources list.
{: shortdesc}

Resources that you expect to be eligible for migration are not listed under the migration task in {{site.data.keyword.mh_short}}, or the eligible resource count is fewer than expected.
{: tsSymptoms}

{{site.data.keyword.mh_short}} identifies eligible resources based on the criteria defined by the service team. A resource may not appear if it does not match the query criteria, if it is in a state that makes it ineligible (for example, already migrated, deprovisioned, or in an error state), or if the resource belongs to a different account.
{: tsCauses}

Try the following steps:

1. Confirm that the resources are provisioned in the same account you are currently viewing in {{site.data.keyword.mh_short}}.
1. Check the resource state in the {{site.data.keyword.cloud_notm}} resource list. Resources in error, suspended, or deprovisioned states may not appear as eligible.
1. Review the migration task description for any eligibility criteria that your resources must meet.
1. If you believe a resource should be eligible but is not shown, contact the service team listed in the migration task or see [Migration help](/docs/migration?topic=migration-help).
{: tsResolve}
