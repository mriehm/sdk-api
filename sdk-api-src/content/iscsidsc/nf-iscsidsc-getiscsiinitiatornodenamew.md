---
UID: NF:iscsidsc.GetIScsiInitiatorNodeNameW
title: GetIScsiInitiatorNodeNameW function (iscsidsc.h)
description: The GetIscsiInitiatorNodeName function retrieves the common initiator node name that is used when establishing sessions from the local machine.
old-location: iscsidisc\getiscsiinitiatornodename.htm
tech.root: iSCSIDisc
ms.assetid: 592d9cd8-5944-479c-ba21-7cf911e0a5b9
ms.date: 12/05/2018
ms.keywords: GetIScsiInitiatorNodeNameW, GetIscsiInitiatorNodeName, GetIscsiInitiatorNodeName function [iSCSI Discovery Library API], GetIscsiInitiatorNodeNameA, GetIscsiInitiatorNodeNameW, iscsidisc.getiscsiinitiatornodename, iscsidsc/GetIscsiInitiatorNodeName, iscsidsc/GetIscsiInitiatorNodeNameA, iscsidsc/GetIscsiInitiatorNodeNameW
ms.topic: function
f1_keywords:
- iscsidsc/GetIscsiInitiatorNodeName
dev_langs:
- c++
req.header: iscsidsc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: GetIscsiInitiatorNodeNameW (Unicode) and GetIscsiInitiatorNodeNameA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Iscsidsc.lib
req.dll: Iscsidsc.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Iscsidsc.dll
api_name:
- GetIscsiInitiatorNodeName
- GetIscsiInitiatorNodeNameA
- GetIscsiInitiatorNodeNameW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# GetIScsiInitiatorNodeNameW function


## -description


The <b>GetIscsiInitiatorNodeName</b> function retrieves the common initiator node name that is used when establishing sessions from the local machine.


## -parameters




### -param InitiatorNodeName

A caller-allocated buffer that, on output, receives the node name. The buffer must be large enough to hold <b>MAX_ISCSI_NAME_LEN+1</b> bytes. 


## -returns



Returns ERROR_SUCCESS if the operation succeeds and the appropriate Win32 or iSCSI error code if the operation fails.





## -remarks



All initiator Host Bus Adapters, both software and hardware, use the same node name when establishing sessions.



