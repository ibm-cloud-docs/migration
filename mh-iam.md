---

copyright:
  years: 2026

lastupdated: "2026-11-02"

keywords: migration hub IAM, IAM permissions, resource controller access, identity access management, migration hub access, IAM roles, migration hub authentication, authorization

subcollection: migration

content-type: conref

---

{{site.data.keyword.attribute-definition-list}}

# Understanding IAM resource visibility in IBM Cloud Migration Hub
{: #mh-iam}


IBM Cloud {{site.data.keyword.mh_short}} uses the same [{{site.data.keyword.iamlong}} (IAM)](/docs/get-coding?topic=get-coding-iam) permissions and access controls as the Resource Controller. No additional IAM configuration is required.
{: shortdesc}

Services that migrate to the Resource Controller bring their existing IAM setup with them. For the full list of required IAM roles and actions, see [IAM and the Resource Controller](/docs/get-coding?topic=get-coding-iam-rc).

## IAM permissions for {{site.data.keyword.mh_short}}
{: #mh-iam-permissions}

Any user or service ID that has the required IAM roles to interact with the Resource Controller can view all the assets in {{site.data.keyword.mh_short}}.

To view assets in {{site.data.keyword.mh_short}}, ensure you have the following permissions:

| Service | Resources | Role |
| ------- | --------- | ---- |
| `All Identity and Access enabled services` | All | Viewer |
| `Resource group only` | All resource groups in the account | Viewer |
{: caption="Permissions required to view assets" caption-side="bottom"}

### Additional persmissions for compute servers
{: #access-compute}

To view the assets for compute servers, you must have the following permissions:
- **View Hardware Details**
- **View Virtual Dedicated Host Details**
- **View Virtual Server Details**

Also, ensure that you have access to the respective devices and servers.

If you do not have these permissions, {{site.data.keyword.mh_short}} redirects you to the {{site.data.keyword.cloud_notm}} console.
{: note}
