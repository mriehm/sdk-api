---
UID: NF:tokenbinding.TokenBindingDeleteBinding
title: TokenBindingDeleteBinding function (tokenbinding.h)
description: Deletes the token binding key that is associated with the specified target string.
old-location: security\tokenbindingdeletebinding.htm
tech.root: SecCNG
ms.assetid: 4258CC92-580E-403C-9AE4-4BB726255464
ms.date: 12/05/2018
ms.keywords: TokenBindingDeleteBinding, TokenBindingDeleteBinding function [Security], security.tokenbindingdeletebinding, tokenbinding/TokenBindingDeleteBinding
ms.topic: function
f1_keywords:
- tokenbinding/TokenBindingDeleteBinding
dev_langs:
- c++
req.header: tokenbinding.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Tokenbinding.lib
req.dll: Tokenbinding.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- tokenbinding.dll
api_name:
- TokenBindingDeleteBinding
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# TokenBindingDeleteBinding function


## -description


Deletes the token binding key that is associated with the specified target string.


## -parameters




### -param targetURL [in]

The target string for which <b>TokenBindingDeleteBinding</b> should delete the associated token binding key.


## -returns



Returns a status code that indicates the success or failure of the function.




## -remarks



You can call <b>TokenBindingDeleteBinding</b> from user mode. 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/tokenbinding/nf-tokenbinding-tokenbindinggeneratebinding">TokenBindingGenerateBinding</a>
 

 

