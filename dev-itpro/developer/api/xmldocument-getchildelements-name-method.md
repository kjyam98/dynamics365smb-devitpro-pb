---
title: "GetChildElements Method"
ms.author: solsen
ms.custom: na
ms.date: 04/01/2019
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: "dynamics365-business-central"
ms.assetid: 620f0e32-eadc-43e9-8f6e-8fc0b12c3aaf
caps.latest.revision: 1
manager: edupont
author: SusanneWindfeldPedersen
redirect_url: /dynamics365/business-central/dev-itpro/developer/methods-auto/library
---
<!--This topic is deprected, see redirection URL-->

 

# GetChildElements Method
Gets a list containing the child elements for this document, in document order.  
```  
ChildElements := XmlDocument.GetChildElements(Name)  
```  
## Parameters
*Name*    
&emsp;Type: [String](../datatypes/devenv-text-data-type.md)  
The fully qualified name of the elements to retrieve.  
  
## Return Value
*ChildElements*  
&emsp;Type: [XmlNodeList](xmlnodelist-class.md)  
  
## See Also
[XmlDocument](xmldocument-class.md)  
[XmlNodeList](xmlnodelist-class.md)  
[HTTP, JSON, TextBuilder, and XML API](../devenv-restapi-overview.md)  
[Getting Started with AL](../devenv-get-started.md)  
[Developing Extensions](../devenv-dev-overview.md)  
