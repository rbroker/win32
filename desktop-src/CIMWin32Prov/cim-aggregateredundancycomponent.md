---
Description: The CIM\_AggregateRedundancyComponent class describes the aggregate physical extent in a storage redundancy group.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 3407e888-e17c-4f65-a33f-056002accbf7
ms.prod: windows-server-dev
ms.technology:
- cimwin32
- windows-management-instrumentation
ms.tgt_platform: multiple
title: CIM\_AggregateRedundancyComponent class
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# CIM\_AggregateRedundancyComponent class

The **CIM\_AggregateRedundancyComponent** class describes the aggregate physical extent in a storage redundancy group.

> \[!Important\]  
> The DMTF (Distributed Management Task Force) CIM (Common Information Model) classes are the parent classes upon which WMI classes are built. WMI currently supports only the [CIM 2.x version schemas](Http://Go.Microsoft.Com/FWLink/p/?LinkID=309367).

 

The following syntax is simplified from Managed Object Format (MOF) code and includes all inherited properties. Properties are listed in alphabetic order, not MOF order.

## Syntax

``` syntax
[Abstract, UUID("{154E66D8-DB35-11d2-85FC-0000F8102E5F}"), AMENDMENT]
class CIM_AggregateRedundancyComponent : CIM_RedundancyComponent
{
  CIM_AggregatePExtent       REF PartComponent;
  CIM_StorageRedundancyGroup REF GroupComponent;
};
```

## Members

The **CIM\_AggregateRedundancyComponent** class has these types of members:

-   [Properties](#properties)

### Properties

The **CIM\_AggregateRedundancyComponent** class has these properties.

<dl> <dt>

**GroupComponent**
</dt> <dd> <dl> <dt>

Data type: **CIM\_StorageRedundancyGroup**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("GroupComponent")
</dt> </dl>

A [**CIM\_StorageRedundancyGroup**](cim-storageredundancygroup.md) that contains the storage redundancy group.

</dd> <dt>

**PartComponent**
</dt> <dd> <dl> <dt>

Data type: **CIM\_AggregatePExtent**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("PartComponent")
</dt> </dl>

A [**CIM\_AggregatePExtent**](cim-aggregatepextent.md) that contains the aggregate physical extent participating in the redundancy group.

</dd> </dl>

## Remarks

The **CIM\_AggregateRedundancyComponent** class is derived from [**CIM\_RedundancyComponent**](cim-redundancycomponent.md).

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

[**CIM\_RedundancyComponent**](cim-redundancycomponent.md)
</dt> </dl>

 

 



