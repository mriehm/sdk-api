---
UID: NN:wmsbuffer.INSSBuffer3
title: INSSBuffer3 (wmsbuffer.h)
description: The INSSBuffer3 interface enhances the INSSBuffer interface by adding the ability to set and retrieve single properties for a sample.
old-location: wmformat\inssbuffer3.htm
tech.root: wmformat
ms.assetid: 3ebf80d0-b5b0-4024-805d-e0a3855574bf
ms.date: 12/05/2018
ms.keywords: INSSBuffer3, INSSBuffer3 interface [windows Media Format], INSSBuffer3 interface [windows Media Format],described, INSSBuffer3Interface, wmformat.inssbuffer3, wmsbuffer/INSSBuffer3
ms.topic: interface
f1_keywords:
- wmsbuffer/INSSBuffer3
dev_langs:
- c++
req.header: wmsbuffer.h
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
- wmsbuffer.h
api_name:
- INSSBuffer3
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# INSSBuffer3 interface


## -description



The <b>INSSBuffer3</b> interface enhances the <a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer">INSSBuffer</a> interface by adding the ability to set and retrieve single properties for a sample. This interface inherits its functionality from the <b>INSSBuffer2</b> interface, which inherits functionality from <b>INSSBuffer</b>. <b>INSSBuffer2</b> is not documented separately in this documentation because the two methods it exposes are not implemented at this time.

To obtain a pointer to the <b>INSSBuffer3</b> interface of an existing buffer object, call <b>INSSBuffer::QueryInterface</b>.



The following interfaces can be obtained by using the QueryInterface method of this interface.
<table>
<tr>
<th>Interface</th>
<th>IID</th>
</tr>
<tr>
<td>
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer">INSSBuffer</a>
</td>
<td>IID_INSSBuffer</td>
</tr>
<tr>
<td>
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer2">INSSBuffer2</a>
</td>
<td>IID_INSSBuffer2</td>
</tr>
<tr>
<td>
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer4">INSSBuffer4</a>
</td>
<td>IID_INSSBuffer4</td>
</tr>
</table>
 




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">INSSBuffer3</b> interface inherits from <a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer">INSSBuffer</a>. <b>INSSBuffer3</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>INSSBuffer3</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer3-getproperty">GetProperty</a>
</td>
<td align="left" width="63%">
Retrieves a property for the sample.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer3-setproperty">SetProperty</a>
</td>
<td align="left" width="63%">
Sets a property for the sample.

</td>
</tr>
</table> 


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer">INSSBuffer Interface</a>



<a href="https://docs.microsoft.com/windows/desktop/wmformat/interfaces">Interfaces</a>
 

 

