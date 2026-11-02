---

copyright:
  years: 2026
lastupdated: "2026-09-28"

keywords: ibm cloud migration failed, migration error, migration recovery, migration rollback, migration failure troubleshooting

subcollection: migration

content-type: troubleshoot

---

{{site.data.keyword.attribute-definition-list}}

# Why did my migration fail, and how do I recover?
{: #troubleshoot-migration-failed}
{: troubleshoot}

Learn how to recover from {{site.data.keyword.cloud_notm}} migration failures, including troubleshooting common errors, rollback procedures, and contacting support.
{: shortdesc}

The migration status in {{site.data.keyword.mh_short}} shows a failed or error state, or you received an error during a migration wizard step.
{: tsSymptoms}

Migration failures can occur for several reasons, including insufficient permissions on the target resource, resource configuration incompatibilities between the source and target products, network or service availability issues during execution, or dependency conflicts where a dependent resource must be migrated first.
{: tsCauses}

Try the following steps:

1. Review the error message displayed in the migration wizard or in {{site.data.keyword.mh_short}} for details about what failed.
1. Check whether you have the necessary IAM roles and access policies for both the source and target services.
1. If the error indicates a dependency issue, review the related resources and migrate any dependencies before retrying.
1. If you used a blue-green deployment or parallel deployment strategy, verify that the source environment is still intact and usable while you troubleshoot.
1. Retry the migration after resolving the identified issue. If the wizard supports it, resume from the last successful step rather than restarting from the beginning.
1. If the failure persists, open a [support case](/docs/migration?topic=migration-help) through the {{site.data.keyword.cloud_notm}} console and include the migration topic ID and any error codes shown in {{site.data.keyword.mh_short}}.
{: tsResolve}

If a rollback is required, review the rollback procedures for your specific migration type before taking action. Some migration wizards include rollback functionality; others may require manual steps.
{: note}
