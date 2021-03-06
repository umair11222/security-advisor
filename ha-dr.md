---

copyright:
  years: 2017, 2020
lastupdated: "2020-10-26"

keywords: HA for {{site.data.keyword.security-advisor_short}}, DR for {{site.data.keyword.security-advisor_short}}, high availability for {{site.data.keyword.security-advisor_short}}, disaster recovery for {{site.data.keyword.security-advisor_short}}, failover for {{site.data.keyword.security-advisor_short}}

subcollection: appid

---

{:codeblock: .codeblock}
{:screen: .screen}
{:download: .download}
{:external: target="_blank" .external}
{:faq: data-hd-content-type='faq'}
{:gif: data-image-type='gif'}
{:important: .important}
{:note: .note}
{:pre: .pre}
{:tip: .tip}
{:preview: .preview}
{:deprecated: .deprecated}
{:beta: .beta}
{:term: .term}
{:shortdesc: .shortdesc}
{:script: data-hd-video='script'}
{:support: data-reuse='support'}
{:table: .aria-labeledby="caption"}
{:troubleshoot: data-hd-content-type='troubleshoot'}
{:help: data-hd-content-type='help'}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:tsSymptoms: .tsSymptoms}
{:java: .ph data-hd-programlang='java'}
{:javascript: .ph data-hd-programlang='javascript'}
{:swift: .ph data-hd-programlang='swift'}
{:curl: .ph data-hd-programlang='curl'}
{:video: .video}
{:step: data-tutorial-type='step'}
{:tutorial: data-hd-content-type='tutorial'}


# Understanding high availability and disaster recovery for {{site.data.keyword.security-advisor_short}}
{: #ha-dr}

{{site.data.keyword.security-advisor_short}} is a highly available, regional service that runs in the Dallas (`us-south`) and London (`eu-gb`) regions.

In each supported region, the service runs in several availability zones. The service supports manual cross-regional failover from `us-south` to `us-east` and from `eu-gb` to `eu-de`. A daily backup of data to Cloud Object Storage is done and the backup is kept for 7 days.

If a regional disaster occurs, the available data is restored by {{site.data.keyword.security-advisor_short}} without any action from you.

To learn more about the high availability and disaster recovery standards in {{site.data.keyword.cloud_notm}}, see [How do I ensure zero downtime?](/docs/overview?topic=overview-zero-downtime) or [Service Level Agreements](/docs/overview?topic=overview-slas).


