---
Description: The CIM\_RedundancyComponent class associates a redundancy group composed of managed system elements and indicates that, together, the elements provide redundancy.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 2511ae26-011a-4e0d-ad34-d5fe9c78f0ff
ms.prod: windows-server-dev
ms.technology:
- cimwin32
- windows-management-instrumentation
ms.tgt_platform: multiple
title: CIM\_RedundancyComponent class
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- CIM_RedundancyComponent
- CIM_RedundancyComponent.GroupComponent
- CIM_RedundancyComponent.PartComponent
api_type: 
- DllExport
api_location: 
- CIMWin32.dll
---

# CIM\_RedundancyComponent class

The **CIM\_RedundancyComponent** class associates a redundancy group composed of managed system elements and indicates that, together, the elements provide redundancy. All elements aggregated in a redundancy group should be instantiations of the same object class.

> \[!Important\]  
> The DMTF (Distributed Management Task Force) CIM (Common Information Model) classes are the parent classes upon which WMI classes are built. WMI currently supports only the [CIM 2.x version schemas](Http://Go.Microsoft.Com/FWLink/p/?LinkID=309367).

 

The following syntax is simplified from Managed Object Format (MOF) code and includes all of its inherited properties. Properties are listed in alphabetic order, not MOF order.

## Syntax

``` syntax
[Abstract, UUID("{FB9D6E62-DB36-11d2-85FC-0000F8102E5F}"), AMENDMENT]
class CIM_RedundancyComponent : CIM_Component
{
  CIM_RedundancyGroup      REF GroupComponent;
  CIM_ManagedSystemElement REF PartComponent;
};
```

## Members

The **CIM\_RedundancyComponent** class has these types of members:

-   [Properties](#properties)

### Properties

The **CIM\_RedundancyComponent** class has these properties.

<dl> <dt>

**GroupComponent**
</dt> <dd> <dl> <dt>

Data type: **CIM\_RedundancyGroup**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("GroupComponent")
</dt> </dl>

The **CIM\_RedundancyComponent** association indicates that 'this set of fans' or 'these physical extents' participate in a single redundancy group.

</dd> <dt>

**PartComponent**
</dt> <dd> <dl> <dt>

Data type: **CIM\_ManagedSystemElement**
</dt> <dt>

Access type: Read-only
</dt> </dl>

A [**CIM\_ManagedSystemElement**](cim-managedsystemelement.md) that describes the child element in the association.

This property is inherited from [**CIM\_Component**](cim-component.md).

</dd> </dl>

## Remarks

**CIM\_RedundancyComponent** is derived from [**CIM\_Component**](cim-component.md).

WMI does not implement this class.

This documentation is derived from the CIM class descriptions published by the DMTF. Microsoft may have made changes to correct minor errors, conform to Microsoft SDK documentation standards, or provide more information.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista<br/>                                                                |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                          |
| Namespace<br/>                | Root\\CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## See also

<dl> <dt>

[**CIM\_Component**](cim-component.md)
</dt> </dl>

 

 



