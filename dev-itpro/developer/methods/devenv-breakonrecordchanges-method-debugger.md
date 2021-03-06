---
title: "BREAKONRECORDCHANGES Method (Debugger)"
ms.custom: na
ms.date: 04/01/2019
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
ms.assetid: 5f0cd768-4b6f-4c11-a10a-c67972521916
author: SusanneWindfeldPedersen
manager: edupont
redirect_url: /dynamics365/business-central/dev-itpro/developer/methods-auto/library
---

 

# BREAKONRECORDCHANGES Method (Debugger)
Breaks execution before a change to a record occurs.  
  
## Syntax  
  
```  
[Ok :=] BREAKONRECORDCHANGES(Ok)   
```  
  
#### Parameters  
 *Ok*  
 Type: Boolean  
  
 Specifies whether the debugger should break execution when a change to a record occurs.  
  
 If *Ok* is true, then the debugger breaks before creating, updating, or deleting a record.  
  
## Property Value/Return Value  
 Type: Boolean  
  
 **True** if the debugger breaks when a change occurs in a record; otherwise, **false**.  
  
 If you omit this optional return value and if the break is not set successfully, then a run-time error occurs. If you include the return value, then you must handle any errors.  
 
## See Also  
[BREAK Method (Debugger)](devenv-break-method-debugger.md)  
[AL Methods](../devenv-al-methods.md)
<!-- 
[Breakpoints](Breakpoints.md)   
[BREAK Method \(Debugger\)](devenv-BREAK-Method-Debugger.md)
-->