---
UID: NF:portabledeviceapi.IEnumPortableDeviceObjectIDs.Cancel
title: IEnumPortableDeviceObjectIDs::Cancel (portabledeviceapi.h)
description: The Cancel method cancels a pending operation.
old-location: wpdsdk\ienumportabledeviceobjectids_cancel.htm
tech.root: wpd_sdk
ms.assetid: ecf4644f-299c-46e0-922c-16de35674222
ms.date: 12/05/2018
ms.keywords: Cancel, Cancel method [Windows Portable Devices SDK], Cancel method [Windows Portable Devices SDK],IEnumPortableDeviceObjectIDs interface, IEnumPortableDeviceObjectIDs interface [Windows Portable Devices SDK],Cancel method, IEnumPortableDeviceObjectIDs.Cancel, IEnumPortableDeviceObjectIDs::Cancel, IEnumPortableDeviceObjectIDsCancel, portabledeviceapi/IEnumPortableDeviceObjectIDs::Cancel, wpdsdk.ienumportabledeviceobjectids_cancel
ms.topic: method
f1_keywords:
- portabledeviceapi/IEnumPortableDeviceObjectIDs.Cancel
dev_langs:
- c++
req.header: portabledeviceapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: PortableDeviceGUIDs.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- PortableDeviceGUIDs.lib
- PortableDeviceGUIDs.dll
api_name:
- IEnumPortableDeviceObjectIDs.Cancel
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IEnumPortableDeviceObjectIDs::Cancel


## -description


The <b>Cancel</b> method cancels a pending operation.
      


## -parameters






## -returns



The method returns an 
<b>HRESULT</b>
. Possible values include, but are not limited to, those in the following table.
          
<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The operation was canceled successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_WPD_DEVICE_NOT_OPEN</b></dt>
</dl>
</td>
<td width="60%">
The device is not opened.

</td>
</tr>
</table>
 




## -remarks



This method cancels all pending operations on the current device handle, which corresponds to a session associated with an <a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nn-portabledeviceapi-iportabledevice">IPortableDevice</a> interface. The Windows Portable Devices (WPD) API does not support targeted cancellation of specific operations.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/portabledeviceapi/nn-portabledeviceapi-ienumportabledeviceobjectids">IEnumPortableDeviceObjectIDs Interface</a>
 

 

