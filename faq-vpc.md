---

copyright:
  years: 2019, 2020
lastupdated: "2020-02-21"

subcollection: vpc


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}
{:faq: data-hd-content-type='faq'}
{:support: data-reuse='support'}


# FAQs for VPC
{: #faqs-for-VPC}

## Can I connect my VPC to my other IBM Cloud workloads?  
{: #faq-vpc-0}
{:faq}
{: support}

Yes, you can set up access to your {{site.data.keyword.cloud}} classic infrastructure from one VPC in each region. For more information, see [Setting up access to classic infrastructure](/docs/vpc?topic=vpc-setting-up-access-to-classic-infrastructure).

## Can a subnet's size be changed after it's created?
{: #faq-vpc-1}
{: faq}

No. You cannot change the size of a subnet after it is created.

## What is the limit on the number of characters in a VPC name?
{: #faq-vpc-2}
{: faq}

Currently, the limit is 100. If this limit is exceeded, you might receive an "internal error" message.

## Can any of my VPC resource names begin with a number?
{: #faq-vpc-3}
{: faq}

No, although the name can contain numbers, it must begin with a letter.

## Are there restrictions on what characters I can use in a name?
{: #faq-vpc-4}
{: faq}

Yes, the UI blocks consecutive double dashes, underscores, and periods from being part of a VSI name.

## Can a subnet size be changed after it is created in a VPC?
{: #faq-vpc-5}
{: faq}

No. You cannot change the size of a subnet after you create it in a VPC.

## During the PGW creation, do I need to reserve the FIP, or does the system automatically reserve the FIP? Will I see that Floating IP when I query all of the Floating IPs?
{: #faq-vpc-6}
{: faq}

The VPC API automatically creates a floating IP along with the public gateway if an existing floating IP is not specified. And yes, that floating IP shows up in the list.

## Who enforces that there must be only one public gateway per zone for a VPC?
{: #faq-vpc-7}
{: faq}

The VPC API service enforces this limit.

## How do I obtain the Cloud Resource Name (CRN) for a VPN?
{: #faq-crn}
{: faq}

To obtain the CRN of a VPC, click **Menu** ![Menu icon](../icons/icon_hamburger.svg) > **Resource list** from the {{site.data.keyword.cloud_notm}} console. Expand **VPC Infrastructure** to list your VPCs. Select a VPC and then click 
the **Status** entry to view its details. Use the icon to copy the CRN and paste it where needed.
