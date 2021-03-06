---
title: "GETLASTERRORTEXT Method"
ms.custom: na
ms.date: 04/01/2019
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
ms.assetid: 5cfff72a-fbee-40e5-9e2b-c5f1f920e506
caps.latest.revision: 13
redirect_url: /dynamics365/business-central/dev-itpro/developer/methods-auto/library
---

 

# GETLASTERRORTEXT Method
Gets the text that was included in the last error message that was generated.  

## Syntax  

```  

String := GETLASTERRORTEXT  
```  

## Property Value/Return Value  
 Type: Text  

 The text string that was contained in the last error message that was generated by [!INCLUDE[d365fin_md](../includes/d365fin_md.md)].  

 If no error has occurred, then the method returns an empty string.  

## Remarks  
 If you call the GETLASTERRORTEXT method immediately after you call the CLEARLASTERROR method, then an empty string is returned.  

 The result of the [GETLASTERRORCODE Method](devenv-GETLASTERRORCODE-Method.md)is not translated into the local language. The result of the GETLASTERRORTEXT method is translated into the local language.  

## Example  
 If you call the Codeunit.RUN method to run a codeunit and an error occurs in the codeunit, then  the error is displayed. However, if you also use the return value of the Codeunit.RUN method, then the error is not displayed. In this case, you can use the GETLASTERRORTEXT method to determine whether an error has occurred and to see the text of the last error message that was generated. This example shows how to use the GETLASTERRORTEXT method. This example requires that you create two codeunits. Codeunit 50001 generates an error. Codeunit 50002 runs codeunit 50001 and if an error occurs, then it displays the text of the error.  

```  
// Codeunit 50001  
// OnRun trigger  
ERROR(‘Some error message.’);  

// Codeunit 50002  
// OnRun trigger  
CLEARLASTERROR();  
IF NOT Codeunit.RUN(50001) THEN  
  MESSAGE(‘The last error was: ’ + GETLASTERRORTEXT);  
```  

 In this example, because the IF statement uses the return value of the Codeunit.RUN method, the error from codeunit 50001 is not displayed. Instead, you use the GETLASTERRORTEXT method to display the error.  

 When you run codeunit 50002, the message window displays the following:  

 **The last error was: Some error message.**  

## See Also  
 [Error Handling Methods](devenv-error-handling-methods.md)
