---
UID: NF:wmsdkidl.IWMMediaProps.SetMediaType
title: IWMMediaProps::SetMediaType (wmsdkidl.h)
description: The SetMediaType method specifies the media type.
old-location: wmformat\iwmmediaprops_setmediatype.htm
tech.root: wmformat
ms.assetid: 7a89bf24-6b76-4645-8f39-f1979029d67e
ms.date: 12/05/2018
ms.keywords: IWMMediaProps interface [windows Media Format],SetMediaType method, IWMMediaProps.SetMediaType, IWMMediaProps::SetMediaType, IWMMediaPropsSetMediaType, SetMediaType, SetMediaType method [windows Media Format], SetMediaType method [windows Media Format],IWMMediaProps interface, wmformat.iwmmediaprops_setmediatype, wmsdkidl/IWMMediaProps::SetMediaType
ms.topic: method
f1_keywords:
- wmsdkidl/IWMMediaProps.SetMediaType
dev_langs:
- c++
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 7 SDK, or later versions of the SDK
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
req.lib: Wmvcore.lib; WMStubDRM.lib (if you use DRM)
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Wmvcore.lib
- Wmvcore.dll
- WMStubDRM.lib
- WMStubDRM.dll
api_name:
- IWMMediaProps.SetMediaType
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWMMediaProps::SetMediaType


## -description



The <b>SetMediaType</b> method specifies the media type.




## -parameters




### -param pType [in]

Pointer to the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/wmsdkidl/ns-wmsdkidl-wm_media_type">WM_MEDIA_TYPE</a> structure describing the input, stream, or output.


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
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>pType</i> parameter is <b>NULL</b>, cbFormat is 0 or too large, or pbFormat is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
There is not enough available memory.

</td>
</tr>
</table>
 




## -remarks



It is possible to successfully set a media type in this method that will ultimately be rejected as invalid when the profile is set on the writer. For a list of tests that the writer performs on the profile, see <a href="https://docs.microsoft.com/windows/desktop/api/wmsdkidl/nf-wmsdkidl-iwmwriter-setprofile">IWMWriter::SetProfile</a>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wmsdkidl/nn-wmsdkidl-iwmmediaprops">IWMMediaProps Interface</a>



<a href="https://docs.microsoft.com/windows/desktop/api/wmsdkidl/nf-wmsdkidl-iwmmediaprops-getmediatype">IWMMediaProps::GetMediaType</a>
 

 

