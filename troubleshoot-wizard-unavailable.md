---

copyright:
  years: 2026
lastupdated: "2026-08-25"

keywords: migration hub troubleshooting, migration wizard unavailable, migration wizard disabled, start migration button

subcollection: migration

content-type: troubleshoot

---

{{site.data.keyword.attribute-definition-list}}

# Why can't I start a migration wizard for my resource?
{: #troubleshoot-wizard-unavailable}
{: troubleshoot}

You can see a migration task in {{site.data.keyword.mh_short}} but the option to launch the migration wizard is disabled or unavailable.
{: shortdesc}

A migration task is listed in {{site.data.keyword.mh_short}}, but the **Start migration** button or migration wizard link is disabled or does not respond.
{: tsSymptoms}

Migration wizards are service-specific tools that are launched from within {{site.data.keyword.mh_short}}. The wizard may be unavailable if the service team has not yet published the migration tooling, if the resource does not meet the eligibility criteria, or if a required prerequisite has not been completed.
{: tsCauses}

Try the following steps:

1. Review the migration task details in {{site.data.keyword.mh_short}} for any prerequisite steps that must be completed before the wizard becomes available.
1. Check whether the migration task shows a status that indicates the resource is not yet eligible — for example, if the resource is in a state that must be resolved first.
1. Review the migration timeline in {{site.data.keyword.mh_short}}. Migration materials and tooling become available 60–90 days before the end date. If you are accessing the task early, tooling may not yet be published.
1. Contact the service team referenced in the migration task, or open a [support case](/docs/migration?topic=migration-help) through the {{site.data.keyword.cloud_notm}} console.
{: tsResolve}
