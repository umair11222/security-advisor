---

copyright:
  years: 2017, 2020
lastupdated: "2020-10-05"

keywords: data encryption in {{site.data.keyword.security-advisor_short}}, data storage for {{site.data.keyword.security-advisor_short}}, personal data in {{site.data.keyword.security-advisor_short}}, data deletion for {{site.data.keyword.security-advisor_short}}, data in {{site.data.keyword.security-advisor_short}}, data security in {{site.data.keyword.security-advisor_short}}

subcollection: security-advisor

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




# Securing your data in {{site.data.keyword.security-advisor_short}}
{: #mng-data}

To ensure that you can securely manage your data when you use {{site.data.keyword.security-advisor_full}}, it is important to know exactly what data is stored and encrypted.
{: shortdesc}

## How your data is stored and encrypted in {{site.data.keyword.security-advisor_short}}
{: #data-storage} 

{{site.data.keyword.security-advisor_short}} stores your data in a highly available and secure environment. The service is enabled by default for all {{site.data.keyword.cloud_notm}} accounts and has public endpoints in the Dallas and London locations.

The raw data that is captured by {{site.data.keyword.security-advisor_short}} during use: 

* Does not contain any personally identifiable information.
* Is encrypted at rest and and in transit.
* Is stored in a managed Cloundant database within each region. 

In each region, a highly available Cloudant cluster contains 3 copies of the data. A daily backup of data to Cloud Object Storage is done and the backup is kept for 7 days. In the event of a failure, the data is automatically recovered by {{site.data.keyword.security-advisor_short}}.

## Deleting your data in {{site.data.keyword.security-advisor_short}}
{: #data-deletion}

{{site.data.keyword.security-advisor_short}} deletes all findings data for each account automatically every 90 days. You don't need to take any action to delete findings data that you no longer require or use.

The findings data that is generated by {{site.data.keyword.security-advisor_short}}:

* Is limited to 18,000 findings, approximately 200 per day, for each account in a 90-day period.
* Is monitored; if the findings limit is met before the 90-day limit, 50% of the findings are deleted in a first-in, first-out model. 
* Is purged when the 90-day limit is reached.
* Is deleted automatically when an account is deleted.
* Can be retrieved by using the API and stored for future use or audit purposes.



