---

copyright:
  years: 2026
lastupdated: "2026-10-27"

keywords: ibm cloud migration release notes, migration hub updates, migration hub new features, cloud migration changes

subcollection: migration

content-type: release-note

---

{{site.data.keyword.attribute-definition-list}}

# IBM Cloud Migration Hub release notes
{: #relnotes}

Stay up-to-date with the latest IBM Cloud {{site.data.keyword.mh_short}} updates, new features, and changes to plan and manage your cloud migrations effectively.
{: shortdesc}

## October 2026
{: #migration-oct2026}
{: release-note}

{{site.data.keyword.cloud_notm}} {{site.data.keyword.mh_short}} is now available
:   {{site.data.keyword.mh_short}} is now available in the {{site.data.keyword.cloud_notm}} console as a centralized platform for managing migrations across {{site.data.keyword.cloud_notm}} products and services. It identifies the resources in your account that require action, helps you plan your migration process, and guides you through each step with instructions, documentation, and tooling, including transitions from deprecated services to their modern replacements.

{{site.data.keyword.mh_short}} launches with three migration topics, each focused on moving workloads from Classic infrastructure to VPC:

- **Clusters migration**: Migrate Red Hat OpenShift Kubernetes Service or IBM Kubernetes Service clusters from Classic to VPC-native networking, with guidance on Landing Zone setup, OADP-based workload migration, migration wizard support, and end-to-end testing and validation instructions. To view this migration in the {{site.data.keyword.mh_short}} UI, see [Containers](/migration/clusters/get-started). For more information, see [Migrating from Classic to VPC](/docs/openshift?topic=openshift-vpc-migrate-overview).

- **Compute servers migration**: Migrate Classic virtual server instances (VSIs) to IBM Cloud VPC with profile-matched sizing, image capture and migration guidance, and validated cutover steps covering VPC landing zone setup, security group configuration, and post-migration validation. To view this migration in the {{site.data.keyword.mh_short}} UI, see [Compute servers](/migration/compute-servers/get-started). For more information, see [Classic to VPC Migration](/docs/classic-to-vpc).

- **Data services migration**: Migrate IBM Cloud Databases (ICD) services from Gen 1 (Classic) to Gen 2 (VPC) architecture with engine-specific migration paths, private endpoint configuration, and automated operations. Supports 30,000+ ICD, Cloudant, and Event Streams deployments at no additional cost. To view this migration in the {{site.data.keyword.mh_short}} UI, see [Data services](/migration/data-services/get-started). For more information, see [Overview of Gen 1 (Classic) and Gen 2 (VPC)](/docs/cloud-databases-gen2?topic=cloud-databases-gen2-overview-gen1-gen2).
