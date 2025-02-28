---
UID: NF:bdaiface.IBDA_MUX.GetPidList
title: IBDA_MUX::GetPidList (bdaiface.h)
description: Gets the list of packet identifiers (PIDs) that are enabled to go across the Protected Broadcast Driver Architecture (PBDA) interface.
old-location: mstv\ibda_mux_getpidlist.htm
tech.root: mstv
ms.assetid: 92b13d40-4841-45ce-b232-5e29a93d71c5
ms.date: 12/05/2018
ms.keywords: GetPidList, GetPidList method [Microsoft TV Technologies], GetPidList method [Microsoft TV Technologies],IBDA_MUX interface, IBDA_MUX interface [Microsoft TV Technologies],GetPidList method, IBDA_MUX.GetPidList, IBDA_MUX::GetPidList, bdaiface/IBDA_MUX::GetPidList, mstv.ibda_mux_getpidlist
ms.topic: method
f1_keywords:
- bdaiface/IBDA_MUX.GetPidList
dev_langs:
- c++
req.header: bdaiface.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Bdaiface.idl
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
- bdaiface.h
api_name:
- IBDA_MUX.GetPidList
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IBDA_MUX::GetPidList


## -description


Gets the list of packet identifiers (PIDs) that are enabled to go across the Protected Broadcast Driver Architecture (PBDA) interface.


## -parameters




### -param pulPidListCount [in, out]

On input, specifies the size, in array elements, of the <i>pbPidListBuffer</i> array. On output, receives the number of PIDs.


### -param pbPidListBuffer [in, out]

Pointer to an array of <a href="https://docs.microsoft.com/previous-versions/windows/desktop/mstv/bda-mux-pidlistitem">BDA_MUX_PIDLISTITEM</a> structures. The method fills in the array with the list of PIDs.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>S_OK</b></b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>E_NOT_SUFFICIENT_BUFFER</b></b></dt>
</dl>
</td>
<td width="60%">
The <i>pbPidListBuffer</i> array is too small.

</td>
</tr>
</table>
 




## -remarks



If the <i>pbPidListBuffer</i> array is too small, the method returns <b>E_NOT_SUFFICIENT_BUFFER</b> and sets the required size in the <i>pulPidListCount</i> parameter.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/bdaiface/nn-bdaiface-ibda_mux">IBDA_MUX</a>
 

 

