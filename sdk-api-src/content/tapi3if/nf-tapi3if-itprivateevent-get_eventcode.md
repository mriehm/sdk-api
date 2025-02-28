---
UID: NF:tapi3if.ITPrivateEvent.get_EventCode
title: ITPrivateEvent::get_EventCode (tapi3if.h)
description: The get_EventCode method returns a pointer to a provider-specific event descriptor.
old-location: tapi3\itprivateevent_get_eventcode.htm
tech.root: Tapi
ms.assetid: a66423ca-c0ed-4d1d-bf28-afc59ac5a5d4
ms.date: 12/05/2018
ms.keywords: ITPrivateEvent interface [TAPI 2.2],get_EventCode method, ITPrivateEvent.get_EventCode, ITPrivateEvent::get_EventCode, _tapi3_itprivateevent_get_eventcode, get_EventCode, get_EventCode method [TAPI 2.2], get_EventCode method [TAPI 2.2],ITPrivateEvent interface, tapi3.itprivateevent_get_eventcode, tapi3if/ITPrivateEvent::get_EventCode
ms.topic: method
f1_keywords:
- tapi3if/ITPrivateEvent.get_EventCode
dev_langs:
- c++
req.header: tapi3if.h
req.include-header: Tapi3.h
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
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Tapi3.dll
api_name:
- ITPrivateEvent.get_EventCode
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ITPrivateEvent::get_EventCode


## -description


The 
<b>get_EventCode</b> method returns a pointer to a provider-specific event descriptor.


## -parameters




### -param plEventCode [out]

 Pointer to the provider-specific event descriptor.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>plEventCode</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/tapi3if/nn-tapi3if-itprivateevent">ITPrivateEvent</a>
 

 

