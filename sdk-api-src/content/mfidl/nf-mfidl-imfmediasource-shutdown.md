---
UID: NF:mfidl.IMFMediaSource.Shutdown
title: IMFMediaSource::Shutdown (mfidl.h)
description: Shuts down the media source and releases the resources it is using.
old-location: mf\imfmediasource_shutdown.htm
tech.root: medfound
ms.assetid: c7f890a8-74bd-4418-bb02-a3fee62dec6d
ms.date: 12/05/2018
ms.keywords: IMFMediaSource interface [Media Foundation],Shutdown method, IMFMediaSource.Shutdown, IMFMediaSource::Shutdown, Shutdown, Shutdown method [Media Foundation], Shutdown method [Media Foundation],IMFMediaSource interface, c7f890a8-74bd-4418-bb02-a3fee62dec6d, mf.imfmediasource_shutdown, mfidl/IMFMediaSource::Shutdown
ms.topic: method
f1_keywords:
- mfidl/IMFMediaSource.Shutdown
dev_langs:
- c++
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- mfuuid.lib
- mfuuid.dll
api_name:
- IMFMediaSource.Shutdown
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMFMediaSource::Shutdown


## -description



Shuts down the media source and releases the resources it is using.




## -parameters






## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

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
The method succeeded.

</td>
</tr>
</table>
 




## -remarks



If the application creates the media source, either directly or through the source resolver, the application is responsible for calling <b>Shutdown</b> to avoid memory or resource leaks.

After this method is called, methods on the media source and all of its media streams return MF_E_SHUTDOWN (except for <b>IUnknown</b> methods).




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/mfidl/nn-mfidl-imfmediasource">IMFMediaSource</a>



<a href="https://docs.microsoft.com/windows/desktop/medfound/media-sources">Media Sources</a>
 

 

