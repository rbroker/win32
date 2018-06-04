---
title: RequestStateChange method of the MSISCSITARGET\_ConcreteJob class
description: Requests that the state of the job be changed to the specified value. The allowed transitions are job specific and vendor specific.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 6e381278-a4a4-4de1-8b12-efb0eaa02d95
ms.prod: windows-server-dev
ms.technology:
- iscsi-target
- windows-management-instrumentation
ms.tgt_platform: multiple
keywords:
- RequestStateChange method iSCSI Software Target API
- RequestStateChange method iSCSI Software Target API , MSISCSITARGET_ConcreteJob class
- MSISCSITARGET_ConcreteJob class iSCSI Software Target API , RequestStateChange method
topic_type:
- apiref
api_name:
- MSISCSITARGET_ConcreteJob.RequestStateChange
api_location:
- SmIScsiTargetProv.dll
api_type:
- COM
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# RequestStateChange method of the MSISCSITARGET\_ConcreteJob class

Requests that the state of the job be changed to the specified value. The allowed transitions are job specific and vendor specific. To invoke this method multiple times could cause earlier requests to be overwritten or to be lost.

This method is inherited from the [**CIM\_ConcreteJob**](https://msdn.microsoft.com/library/cc136808) class.

## Syntax


```mof
uint32 RequestStateChange(
  [in] uint16   RequestedState,
  [in] datetime TimeoutPeriod
);
```



## Parameters

<dl> <dt>

*RequestedState* \[in\]
</dt> <dd>

Specifies the state to which the job should be changed.

<dt>

<span id="Start"></span><span id="start"></span><span id="START"></span>

<span id="Start"></span><span id="start"></span><span id="START"></span>**Start** (2)


</dt> <dd>

Changes the state to Running.

</dd> <dt>

<span id="Suspend"></span><span id="suspend"></span><span id="SUSPEND"></span>

<span id="Suspend"></span><span id="suspend"></span><span id="SUSPEND"></span>**Suspend** (3)


</dt> <dd>

Stops the job temporarily. You can restart the job and possibly enter the Service state while the job is suspended. This value is job-specific.

</dd> <dt>

<span id="Terminate"></span><span id="terminate"></span><span id="TERMINATE"></span>

<span id="Terminate"></span><span id="terminate"></span><span id="TERMINATE"></span>**Terminate** (4)


</dt> <dd>

Stops the job cleanly, save data, preserve the state, and shut down all underlying processes in an orderly manner.

</dd> <dt>

<span id="Kill"></span><span id="kill"></span><span id="KILL"></span>

<span id="Kill"></span><span id="kill"></span><span id="KILL"></span>**Kill** (5)


</dt> <dd>

Stops the job immediately with no requirement to save data or preserve the state.

</dd> <dt>

<span id="Service"></span><span id="service"></span><span id="SERVICE"></span>

<span id="Service"></span><span id="service"></span><span id="SERVICE"></span>**Service** (6)


</dt> <dd>

Puts the job into a vendor-specific Service state. It might be possible to restart the job from this state.

</dd> <dt>

<span id="DMTF_Reserved"></span><span id="dmtf_reserved"></span><span id="DMTF_RESERVED"></span>

<span id="DMTF_Reserved"></span><span id="dmtf_reserved"></span><span id="DMTF_RESERVED"></span>**DMTF Reserved**


</dt> <dd>

Reserved.

</dd> <dt>

<span id="Vendor_Reserved"></span><span id="vendor_reserved"></span><span id="VENDOR_RESERVED"></span>

<span id="Vendor_Reserved"></span><span id="vendor_reserved"></span><span id="VENDOR_RESERVED"></span>**Vendor Reserved**


</dt> <dd>

Reserved.

</dd> </dl> </dd> <dt>

*TimeoutPeriod* \[in\]
</dt> <dd>

Specifies the maximum amount of time that the client expects the transition to the new state to take. The interval format must be used to specify the *TimeoutPeriod* parameter. A value of 0 or a null parameter indicates that the client has no time requirements for the transition.

> [!Note]  
> If the implementation does not support this parameter and this property does not contain 0 or null, the **Use Of Timeout Parameter Not Supported** value must be returned.

 

</dd> </dl>

## Return value

This method returns one of the following values.

<dl> <dt>

**Completed with No Error** (0)
</dt> <dt>

**Not Supported** (1)
</dt> <dt>

**Unknown/Unspecified Error** (2)
</dt> <dt>

**Can NOT complete within Timeout Period** (3)
</dt> <dt>

**Failed** (4)
</dt> <dt>

**Invalid Parameter** (5)
</dt> <dt>

**In Use** (6)
</dt> <dt>

**DMTF Reserved** (7 4095)
</dt> <dt>

**Method Parameters Checked - Transition Started** (4096)
</dt> <dt>

**Invalid State Transition** (4097)
</dt> <dt>

**Use of Timeout Parameter Not Supported** (4098)
</dt> <dt>

**Busy** (4099)
</dt> <dt>

**Method Reserved** (4100 32767)
</dt> <dt>

**Vendor Specific** (32768 65535)
</dt> </dl>

## Requirements



|                                     |                                                                                                  |
|-------------------------------------|--------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                        |
| Minimum supported server<br/> | Windows Server 2012 R2<br/>                                                                |
| Namespace<br/>                | Root\\CIMv2\\Storage\\iScsiTarget<br/>                                                     |
| MOF<br/>                      | <dl> <dt>SmIscsiTarget.mof</dt> </dl>     |
| DLL<br/>                      | <dl> <dt>SmIScsiTargetProv.dll</dt> </dl> |



## See also

<dl> <dt>

[**MSISCSITARGET\_ConcreteJob**](msiscsitarget-concretejob.md)
</dt> </dl>

 

 




