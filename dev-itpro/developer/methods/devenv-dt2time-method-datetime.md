---
title: "DT2TIME Method (DateTime)"
ms.custom: na
ms.date: 04/01/2019
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
ms.assetid: 174d53c4-7f71-4e3b-800e-d8d729552123
author: SusanneWindfeldPedersen
manager: edupont
redirect_url: /dynamics365/business-central/dev-itpro/developer/methods-auto/library
---

 

# DT2TIME Method (DateTime)
Gets the time part of a DateTime object.  
  
## Syntax  
  
```  
  
Time := DT2TIME(Datetime)  
```  
  
#### Parameters  
 *Datetime*  
 Type: DateTime  
  
 The DateTime of which to return the time part.  
  
## Property Value/Return Value  
 Type: Time  
  
 The time part of the DateTime object.  
  
## Remarks  
 If *Datetime* is undefined, then this method returns an undefined time.  
  
## See Also  
 [DateTime Methods](devenv-DateTime-Methods.md)