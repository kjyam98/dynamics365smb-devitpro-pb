---
title: "FilterGroup Method"
ms.author: solsen
ms.custom: na
ms.date: 04/01/2019
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: "dynamics365-business-central"
author: solsen
---
[//]: # (START>DO_NOT_EDIT)
[//]: # (IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT.)
[//]: # (Any modifications should be made in the .xml files in the ModernDev repo.)
# FilterGroup Method
Changes the filter group that is being applied to the table. You can also use this method to return the number of the current filtergroup. You cannot return the number of the filtergroup and set a new filtergroup at the same time.


## Syntax
```
[Group := ]  RecordRef.FilterGroup([NewGroup: Integer])
```
> [!NOTE]  
> This method can be invoked using property access syntax.  
## Parameters
*RecordRef*  
&emsp;Type: [RecordRef](recordref-data-type.md)  
An instance of the [RecordRef](recordref-data-type.md) data type.  

*NewGroup*  
&emsp;Type: [Integer](../integer/integer-data-type.md)  
The ID of the new filter group.  


## Return Value
*Group*  
&emsp;Type: [Integer](../integer/integer-data-type.md)  
The ID of the filter group.  


[//]: # (IMPORTANT: END>DO_NOT_EDIT)

## Remarks  
 A filtergroup can contain a filter for a RecordRef that has been set earlier with SETFILTER or SETRANGE. The total filter applied is the combination of all the filters set in all the filtergroups.  
  
 This method works the same way as the [FILTERGROUP Method \(Record\)](../../methods/devenv-filtergroup-method-record.md).  
  
## Example  
 The following example determines the filtergroup that is set on the Customer table and then changes filtergroup to 1, which is the filtergroup that is applied globally to the entire application. The code starts by opening the Customer table with a RecordRef variable. The [SETRECFILTER Method \(RecordRef\)](../../methods/devenv-setrecfilter-method-recordref.md) sets the values in the current key of the current record as a record filter. This filter is a standard filtergroup so it has a filtergroup number of 0. Then the FILTERGROUP method returns the number for the filtergroup. This filtergroup is a standard filter so the return value is 0. This value is stored in the varOrigGroup variable and displayed in a message box. The FILTERGROUP method changes the filtergroup to 1, which is the number for the global filtergroup. The new value is stored in the varCurrGroup variable and displayed in a message box. This example requires that you create the following global variables and text constants.  
  
|Variable name|DataType|  
|-------------------|--------------|  
|MyRecordRef|RecordRef|  
|varOrigGroup|Integer|  
|varCurrGroup|Integer|  
  
|Text constant name|ENU value|  
|------------------------|---------------|  
|Text000|The original filtergroup is: %1|  
|Text001|The current filtergroup is: %1|  
  
```  
  
MyRecordRef.OPEN(DATABASE::Customer);  
MyRecordRef.SETRECFILTER;  
varOrigGroup := MyRecordRef.FILTERGROUP;  
MESSAGE(Text000, varOrigGroup);  
varCurrGroup := MyRecordRef.FILTERGROUP(1);  
MESSAGE(Text001, varCurrGroup);  
```  
  
## See Also
[RecordRef Data Type](recordref-data-type.md)  
[Getting Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)