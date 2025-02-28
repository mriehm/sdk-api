---
UID: NF:mpeg2psiparser.ICAT.RegisterForNextTable
title: ICAT::RegisterForNextTable (mpeg2psiparser.h)
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
old-location: mstv\icat_registerfornexttable.htm
tech.root: mstv
ms.assetid: 17d77207-253f-48e2-a7ec-3bcc549d2d5e
ms.date: 12/05/2018
ms.keywords: ICAT interface [Microsoft TV Technologies],RegisterForNextTable method, ICAT.RegisterForNextTable, ICAT::RegisterForNextTable, ICATRegisterForNextTable, RegisterForNextTable, RegisterForNextTable method [Microsoft TV Technologies], RegisterForNextTable method [Microsoft TV Technologies],ICAT interface, mpeg2psiparser/ICAT::RegisterForNextTable, mstv.icat_registerfornexttable
ms.topic: method
f1_keywords:
- mpeg2psiparser/ICAT.RegisterForNextTable
dev_langs:
- c++
req.header: mpeg2psiparser.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- mpeg2psiparser.h
api_name:
- ICAT.RegisterForNextTable
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ICAT::RegisterForNextTable


## -description



This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        



The <b>RegisterForNextTable</b> method registers the client to be notified when a <i>next</i> table arrives that will replace the current table.


## -parameters




### -param hNextTableAvailable [in]

Handle to an event created by the caller. The object signals the event when the <i>next</i> table arrives. When the event is signaled, call the <a href="https://docs.microsoft.com/windows/desktop/api/mpeg2psiparser/nf-mpeg2psiparser-icat-getnexttable">ICAT::GetNextTable</a> method to retrieve the table.


## -returns



The method returns an <b>HRESULT</b>. Possible values include those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_ACCESSDENIED</b></dt>
</dl>
</td>
<td width="60%">
This table is already a <i>next</i> table.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid argument; <i>hNextTableAvailable</i> cannot be <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MPEG2_E_ALREADY_INITIALIZED</b></dt>
</dl>
</td>
<td width="60%">
The method has already been called.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -remarks



This method applies only to <i>current</i> tables. Otherwise, the method returns E_ACCESSDENIED.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/mpeg2psiparser/nn-mpeg2psiparser-icat">ICAT Interface</a>
 

 

