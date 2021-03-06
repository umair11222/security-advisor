---

copyright:
  years: 2017, 2020
lastupdated: "2020-09-21"

keywords: Centralized security, security management, alerts, security risk, insights, threat detection

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



# Twistlock
{: #setup-twistlock}

You can prevent risk by stopping the deployment of vulnerable images in your environment. With automated and custom policy enforcement, [Twistlock](https://www.twistlock.com){: external} offers complete control at every stage of the application lifecycle.
{: shortdesc}

When you configure the business partner connection, two cards are created in your dashboard that summarize the findings from Twistlock.

**Twistlock Runtime** introduces two Key Performance Indicators (KPIs):

* Total incidents and audits: Findings that are related to incidents or audits on your cloud-native workloads.
* Total firewall audits: Findings that are related to issues with your firewall.

**Twistlock vulnerabilities** introduce one KPI:

* Total images with new vulnerabilities: Findings that are related to vulnerabilities found in your container images.


## Before you begin
{: #twistlock-before}

Before you start integrating business partners, be sure that you have the following prerequisites.

* Ensure that you have an account with the business partner that you want to integrate.
* Ensure that you have the required permissions to generate the integration URL for the business partner service.
* Ensure that you have IAM administrator access {{site.data.keyword.security-advisor_short}}.


## Integration wizard
{: #wizard-twistlock}

As an administrator with the needed permissions in both the {{site.data.keyword.cloud_notm}} and business partner accounts, you can use the integration wizard to quickly get up and running with Twistlock. The wizard has four basic steps:

* Establish trust and associate your {{site.data.keyword.cloud_notm}} and business partner accounts
* Copy the required information such as credentials and URLs between the accounts
* Install the business partner's finding metadata into {{site.data.keyword.security-advisor_short}}
* Validate the pairing by posting a finding from the business partner into {{site.data.keyword.security-advisor_short}}



## Configuring Twistlock
{: #configure-twistlock}

1. In the {{site.data.keyword.security-advisor_short}} dashboard, navigate to **Integrations > Partner Integrations** and select **Twistlock** from the options provided.

2. Click **Yes, connect my account to {{site.data.keyword.security-advisor_short}}**.

  If you don't already have an account, click **No, help me create an account > Create an account**. You can fill out your information and the Twistlock sales team will contact you to get started.
  {: note}

3. Give your connection a name. Be sure that the name is unique to your account and that you use only alpha-numeric characters, space, or a hyphen.

4. Optional: If you don't already have a configuration URL, click **Generate registration URL** to go to the Twistlock documentation and learn how to create the URL. Be sure that you have the Twistlock token that comes with your license to gain access to the docs.

5. In the Twistlock dashboard, navigate to the **Manage > Alerts** tab and click **Add profile**.

6. Select **{{site.data.keyword.security-advisor_short}}** from the **Provider** drop down.

7. Click **Copy** to use the provided configuration URL.

8. Back in the {{site.data.keyword.security-advisor_short}} dashboard, paste the URL in the **Enter the Twistlock configuration URL** box.

9. Click **Connect Partner**.



## Verifying the connection
{: #twistlock-verify}

1. In the {{site.data.keyword.security-advisor_short}} dashboard, check to see whether the Twistlock cards are displaying as expected.

2. In the Twistlock dashboard, refresh the **Alerts** tab. The {{site.data.keyword.security-advisor_short}} connection shows. Open the connection.

3. Verify that the alert types that you want to be notified of are  checked and then click **Verify** to ensure that the connection is complete.
