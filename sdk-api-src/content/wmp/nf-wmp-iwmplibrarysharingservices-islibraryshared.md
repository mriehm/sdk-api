---
UID: NF:wmp.IWMPLibrarySharingServices.isLibraryShared
title: IWMPLibrarySharingServices::isLibraryShared (wmp.h)
description: The isLibraryShared method retrieves a value indicating whether the user's library is shared.
old-location: wmp\iwmplibrarysharingservices_islibraryshared.htm
tech.root: WMP
ms.assetid: fc0a1396-5b43-43dd-9e0d-b5b3a8cf5cdd
ms.date: 12/05/2018
ms.keywords: IWMPLibrarySharingServices interface [Windows Media Player],isLibraryShared method, IWMPLibrarySharingServices.isLibraryShared, IWMPLibrarySharingServices::isLibraryShared, IWMPLibrarySharingServicesisLibraryShared, isLibraryShared, isLibraryShared method [Windows Media Player], isLibraryShared method [Windows Media Player],IWMPLibrarySharingServices interface, wmp.iwmplibrarysharingservices_islibraryshared, wmp/IWMPLibrarySharingServices::isLibraryShared
ms.topic: method
f1_keywords:
- wmp/IWMPLibrarySharingServices.isLibraryShared
dev_langs:
- c++
req.header: wmp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Media Player 11.
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
req.dll: Wmp.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- wmp.dll
api_name:
- IWMPLibrarySharingServices.isLibraryShared
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWMPLibrarySharingServices::isLibraryShared


## -description



The <b>isLibraryShared</b> method retrieves a value indicating whether the user's library is shared.




## -parameters




### -param pvbShared [out]

Pointer to a <b>VARIANT_BOOL</b> that receives the result. <b>VARIANT_TRUE</b> indicates that the user's library is currently shared.


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



<b>Windows Media Player 10 Mobile:</b> This method is not supported.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wmp/nn-wmp-iwmplibrarysharingservices">IWMPLibrarySharingServices Interface</a>
 

 

