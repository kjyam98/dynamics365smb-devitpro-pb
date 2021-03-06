---
title: "BREAK Method (Debugger)"
ms.custom: na
ms.date: 04/01/2019
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
ms.assetid: e0b2c3ac-950b-44f5-a291-268ab70d8a96
author: SusanneWindfeldPedersen
manager: edupont
redirect_url: /dynamics365/business-central/dev-itpro/developer/methods-auto/library
---

 

# BREAK Method (Debugger)
Breaks code execution of a debugging session.  
  
## Syntax  
  
```  
[Ok :=] BREAK   
```  
  
## Property Value/Return Value  
Type: Boolean  
  
**True** if a breakpoint is set in the debugging session; otherwise, **false**.  
  
If you omit this optional return value and if the break is not set successfully, then a run-time error occurs. If you include the return value, then you must handle any errors.  

## See Also  
[AL Methods](../devenv-al-methods.md)  
[BREAKONERROR Method (Debugger)](devenv-breakonerror-method-debugger.md) 
<!--
[Breakpoints](devenv-Breakpoints.md)   
[How to: Break on the Next Statement](How-to--Break-on-the-Next-Statement.md)   
[How to: Manage Breakpoints from the Development Environment](How-to--Manage-Breakpoints-from-the-Development-Environment.md)
-->