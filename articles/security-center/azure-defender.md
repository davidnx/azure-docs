---
title: Overview of Azure Defender and the available plans
description: Learn about Azure Defender's plans, protections, and alerts. Then proceed to enable Azure Defender on your subscriptions. 
author: memildin
ms.author: memildin
ms.date: 9/22/2020
ms.topic: conceptual
ms.service: security-center
manager: rkarlin

---

# Introduction to Azure Defender

Azure Security Center's features cover the two broad pillars of cloud security:

- **Cloud security posture management (CSPM)**
- **Cloud workload protection (CWP)**

The CSPM features of Security Center, such as secure score, detection of security misconfigurations in your Windows and Linux Azure machines, are all part of the free Security Center experience available to all Azure users. Use these CSPM features to strengthen your posture and ensure regulatory compliance.

**Azure Defender** is the cloud workload protection platform (CWPP) integrated within Security Center for advanced, intelligent, protection of your Azure and hybrid workloads.

This is the Azure Defender dashboard in Azure Security Center:

:::image type="content" source="./media/azure-defender/sample-defender-dashboard.png" alt-text="An example of the Azure Defender dashboard" lightbox="./media/azure-defender/sample-defender-dashboard.png":::

## What resource types can Azure Defender secure?

Azure Defender provides security alerts and advanced threat protection for virtual machines, SQL databases, containers, web applications, your network, and more.

When you enable Azure Defender from the **Pricing and settings** area of Azure Security Center, the following Defender plans are all enabled simultaneously and provide comprehensive defenses for the compute, data, and service layers of your environment:

- [Azure Defender for servers](defender-for-servers-introduction.md)
- [Azure Defender for App Service](defender-for-app-service-introduction.md)
- [Azure Defender for Storage](defender-for-storage-introduction.md)
- [Azure Defender for SQL](defender-for-sql-introduction.md)
- [Azure Defender for IoT](defender-for-iot-introduction.md)
- [Azure Defender for Kubernetes](defender-for-kubernetes-introduction.md)
- [Azure Defender for container registries](defender-for-container-registries-introduction.md)
- [Azure Defender for Key Vault](defender-for-key-vault-introduction.md)

Each of these plans is explained separately in the Security Center documentation.


## Hybrid cloud protection

As well as defending your Azure environment, you can add Azure Defender capabilities to your hybrid cloud environment:

- Protect your non-Azure servers
- Protect your virtual machines in other clouds (such as AWS and GCP)
- Protect your IoT devices

You'll get customized threat intelligence and prioritized alerts according to your specific environment so that you can focus on what matters the most​

Deploy [Azure Arc](https://azure.microsoft.com/services/azure-arc/) and enable Azure Defender to extend protection to on-premises and multi-cloud virtual machines and SQL databases. Azure Arc for servers is a free service, but services that are used on Arc enabled servers, for example Azure Defender, will be charged as per the pricing for that service.

[Learn more about Azure Arc](https://docs.microsoft.com/azure/azure-arc/overview).


## Azure Defender alerts 

When Azure Defender detects a threat in any area of your environment, it generates an alert. These alerts describe details of the affected resources, suggested remediation steps, and in some cases an option to trigger a logic app in response.

Whether an alert is generated by Security Center, or received by Security Center from an integrated  security product, you can export it. To export your alerts to Azure Sentinel, any third-party SIEM, or any other external tool, follow the instructions in [Exporting alerts to a SIEM](continuous-export.md).

> [!NOTE]
> Alerts from different sources might take different amounts of time to appear. For example, alerts that require analysis of network traffic might take longer to appear than alerts related to suspicious processes running on virtual machines.


## Azure Defender advanced protection capabilities

Azure Defender uses advanced analytics for tailored recommendations related to your resources. 

Protections include securing the management ports of your VMs with just-in-time access and adaptive application controls to create allow lists for what apps should and shouldn't run on your machines. 

Use the advanced protection tiles in the Azure Defender dashboard to monitor and configure each of these protections. 

## Vulnerability assessment and management

Azure Defender includes vulnerability scanning for your virtual machines and container registries at no extra cost. The scanners are powered by Qualys but you don't need a Qualys license or even a Qualys account - everything's handled seamlessly inside Security Center. 

Review the findings from these vulnerability scanners and respond to them all from within Security Center. This brings Security Center closer to being the single pane of glass for all of your cloud security efforts.

Learn more on the following pages:

- [Security Center's integrated vulnerability assessment solution for Azure virtual machines](deploy-vulnerability-assessment-vm.md)
- [Identify vulnerabilities in images in Azure container registries](defender-for-container-registries-usage.md#identify-vulnerabilities-in-images-in-other-container-registries)



## Next steps

In this article, you learned about the benefits of Azure Defender. 

> [!div class="nextstepaction"]
> [Enable Azure Defender](security-center-pricing.md)