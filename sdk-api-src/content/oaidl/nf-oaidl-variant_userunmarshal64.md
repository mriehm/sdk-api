---
UID: NF:oaidl.VARIANT_UserUnmarshal64
title: VARIANT_UserUnmarshal64 function (oaidl.h)
description: Unmarshals a VARIANT object from the RPC buffer.
old-location: automat\variant_userunmarshal64.htm
tech.root: automat
ms.assetid: c4539285-20c2-4eda-acbc-1f1a80cad07b
ms.date: 12/05/2018
ms.keywords: VARIANT_UserUnmarshal64, VARIANT_UserUnmarshal64 function [Automation], automat.variant_userunmarshal64, oaidl/VARIANT_UserUnmarshal64
ms.topic: function
f1_keywords:
- oaidl/VARIANT_UserUnmarshal64
dev_langs:
- c++
req.header: oaidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: OleAut32.lib
req.dll: OleAut32.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- OleAut32.dll
api_name:
- VARIANT_UserUnmarshal64
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# VARIANT_UserUnmarshal64 function


## -description


Unmarshals a <a href="https://docs.microsoft.com/windows/desktop/api/oaidl/ns-oaidl-variant">VARIANT</a> object from the RPC buffer.


## -parameters




### -param arg1 [in]

The data used by RPC.


### -param arg2 [in]

The current buffer. This pointer may or may not be aligned on entry.


### -param arg3 [out]

The object.


## -returns



The value obtained from the returned <b>HRESULT</b> value is one of the following.

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
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG
</b></dt>
</dl>
</td>
<td width="60%">
The <i>pVariant</i> parameter is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_X_BAD_STUB_DATA
</b></dt>
</dl>
</td>
<td width="60%">
The stub data for the buffer size is incorrect.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DISP_E_BADVARTYPE
</b></dt>
</dl>
</td>
<td width="60%">
The input parameter is not a valid type of variant.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory for this function to perform.

</td>
</tr>
</table>
 



