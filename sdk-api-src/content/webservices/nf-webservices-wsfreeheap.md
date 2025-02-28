---
UID: NF:webservices.WsFreeHeap
title: WsFreeHeap function (webservices.h)
description: This frees the heap object, and the memory associated with any allocations made on it using WsAlloc.
old-location: wsw\wsfreeheap.htm
tech.root: wsw
ms.assetid: ec643915-8c4b-4916-b390-d6ca043350db
ms.date: 12/05/2018
ms.keywords: WsFreeHeap, WsFreeHeap function [Web Services for Windows], webservices/WsFreeHeap, wsw.wsfreeheap
ms.topic: function
f1_keywords:
- webservices/WsFreeHeap
dev_langs:
- c++
req.header: webservices.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WebServices.lib
req.dll: WebServices.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- WebServices.dll
api_name:
- WsFreeHeap
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# WsFreeHeap function


## -description


This frees the heap object, and the memory associated with any allocations 
                made on it using <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wsalloc">WsAlloc</a>.
            


## -parameters




### -param heap [in]

The heap to free.  This must be a valid heap object that was returned
                    from <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wscreateheap">WsCreateHeap</a>.  This parameter may not be <b>NULL</b>.
                


## -returns



This function does not return a value.



