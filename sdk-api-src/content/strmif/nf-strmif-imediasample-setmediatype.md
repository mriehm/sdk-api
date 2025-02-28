---
UID: NF:strmif.IMediaSample.SetMediaType
title: IMediaSample::SetMediaType (strmif.h)
description: The SetMediaType method sets the media type for the sample.
old-location: dshow\imediasample_setmediatype.htm
tech.root: DirectShow
ms.assetid: 5be0997a-ae70-45fb-94e4-cb5e0a36d71a
ms.date: 12/05/2018
ms.keywords: IMediaSample interface [DirectShow],SetMediaType method, IMediaSample.SetMediaType, IMediaSample::SetMediaType, IMediaSampleSetMediaType, SetMediaType, SetMediaType method [DirectShow], SetMediaType method [DirectShow],IMediaSample interface, dshow.imediasample_setmediatype, strmif/IMediaSample::SetMediaType
ms.topic: method
f1_keywords:
- strmif/IMediaSample.SetMediaType
dev_langs:
- c++
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Strmiids.lib
- Strmiids.dll
api_name:
- IMediaSample.SetMediaType
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMediaSample::SetMediaType


## -description



The <code>SetMediaType</code> method sets the media type for the sample.




## -parameters




### -param pMediaType

Pointer to an <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/strmif/ns-strmif-am_media_type">AM_MEDIA_TYPE</a> structure that specifies the media type.


## -returns



Returns an <b>HRESULT</b> value. Possible values include those shown in the following table.

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
Success

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory

</td>
</tr>
</table>
 




## -remarks



By default, every sample has the same media type as the previous sample. (The pin connection determines the original media type.) Call this method to make limited changes to the media type, such as changing the palette. To make a significant change to the media type, the pins might need to reconnect and renegotiate the media type.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/DirectShow/error-and-success-codes">Error and Success Codes</a>



<a href="https://docs.microsoft.com/windows/desktop/api/strmif/nn-strmif-imediasample">IMediaSample Interface</a>
 

 

