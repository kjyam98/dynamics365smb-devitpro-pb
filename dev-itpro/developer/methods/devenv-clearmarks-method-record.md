---
title: "CLEARMARKS Method (Record)"
ms.custom: na
ms.date: 04/01/2019
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
ms.assetid: 52b76918-c0b4-48b6-9635-0ac38308613d
author: SusanneWindfeldPedersen
manager: edupont
redirect_url: /dynamics365/business-central/dev-itpro/developer/methods-auto/library
---

 

# CLEARMARKS Method (Record)
Removes all the marks from a record.  
  
## Syntax  
  
```  
  
Record.CLEARMARKS  
```  
  
#### Parameters  
 *Record*  
 Type: Record  
  
 The record from which you want to remove all marks.  
  
## Example  
 This example requires that you create a CustomerRec variable that has data type of Record and subtype of Customer.  
  
```  
CustomerRec.CLEARMARKS  
```  
  
## See Also  
 [Record Data Type](../datatypes/devenv-Record-Data-Type.md)