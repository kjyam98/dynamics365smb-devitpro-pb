---
title: "Upgrading to Microsoft Dynamics 365 Business Central Online"
ms.custom: na
ms.reviewer: edupont
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.author: jswymer
author: jswymer
ms.service: "dynamics365-business-central"
ms.date: 04/01/2019
---
# Upgrading to [!INCLUDE[prodlong](../developer/includes/prodlong.md)] Online

If you want to move your current solution to [!INCLUDE[prodshort](../developer/includes/prodshort.md)] online, the path depends on your current solution. In all cases, it's a matter of migration rather than upgrade due to the nature of online services. The core scenario is to import existing data to an empty company in a [!INCLUDE[prodshort](../developer/includes/prodshort.md)] online tenant. For more information, see [Take prospects and customers online](../deployment/deployment.md#take-prospects-and-customers-online).  

Use the following table to determine the procedures that you must complete for your migration scenario:

|  Scenario  |  Procedures  |
|------------|--------------|
|Upgrade from [!INCLUDE[navnow](../developer/includes/navnow_md.md)]|Upgrading from [!INCLUDE[navnow_md](../developer/includes/navnow_md.md)] to [!INCLUDE[prodshort](../developer/includes/prodshort.md)] online is only partially supported.</br>For more information, see [Upgrading from Dynamics NAV to Business Central online](upgrade-considerations.md#upgrading-from--to--online).|
|Set up a company based on questionnaires|Use RapidStart Services. </br>For more information, see [Setting Up a Company With RapidStart Services](/dynamics365/business-central/admin-set-up-a-company-with-rapidstart?toc=/dynamics365/business-central/dev-itpro/toc.json).|
|Import data from any system|Use Excel or configuration packages to import data. </br>For more information, see [Importing Business Data from Other Finance Systems](/dynamics365/business-central/across-import-data-configuration-packages?toc=/dynamics365/business-central/dev-itpro/toc.json).|
|Import data from Dynamics GP|Use the data migration wizard to import master data. </br>For more information, see [The Dynamics GP Data Migration Extension](/dynamics365/business-central/ui-extensions-dynamicsgp-data-migration?toc=/dynamics365/business-central/dev-itpro/toc.json).|
|Import data from Intuit QuickBooks|Use the data migration wizard to import master data. </br>For more information, see [The QuickBooks Data Migration Extension](/dynamics365/business-central/ui-extensions-quickbooks-data-migration?toc=/dynamics365/business-central/dev-itpro/toc.json).|

## See Also

[Upgrading to [!INCLUDE[prodlong](../developer/includes/prodlong.md)]](upgrading-to-business-central.md)  
[Upgrading to [!INCLUDE[prodlong](../developer/includes/prodlong.md)] On-Premises](upgrading-to-business-central-on-premises.md)  
[The Lifecycle of Apps and Extensions for Business Central](../developer/devenv-app-life-cycle.md)  
[Upgrading Extensions](../developer/devenv-upgrading-extensions.md)  
[Product and Architecture Overview](../deployment/Product-and-Architecture-Overview.md)  
[Deployment](../deployment/Deployment.md)  
