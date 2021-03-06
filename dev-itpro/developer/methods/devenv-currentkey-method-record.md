---
title: "CURRENTKEY Method (Record)"
ms.custom: na
ms.date: 04/01/2019
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
ms.assetid: daf99f50-4833-4e08-8360-a3b63e5139be
author: SusanneWindfeldPedersen
manager: edupont
redirect_url: /dynamics365/business-central/dev-itpro/developer/methods-auto/library
---

 

# CURRENTKEY Method (Record)
Gets the current key of a database table.  
  
## Syntax  
  
```  
  
CurrentKey := Record.CURRENTKEY  
```  
  
#### Parameters  
 *Record*  
 Type: Record  
  
 A record that refers to the table for which you want to find the key that is currently in use.  
  
## Property Value/Return Value  
 Type: Text or code  
  
 The name of the current key of *Record*.  
  
## Example  
 The following example returns the current key that is used in the **Customer** table and displays it in a message box. The MyRecord record is from the **Customer** table. This example requires that you create the following global variables and text constant.  
  
|Variable name|DataType|Subtype|  
|-------------------|--------------|-------------|  
|MyRecord|Record|Customer|  
|CurrentKey|Text|Not applicable|  
  
|Text constant name|ConstValue|  
|------------------------|----------------|  
|Text000|The current key is: %1|  
  
```  
CurrentKey := MyRecord.CURRENTKEY;  
MESSAGE(Text000, CurrentKey);  
```  
  
## See Also  
 [Record Data Type](../datatypes/devenv-Record-Data-Type.md)