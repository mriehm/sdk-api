---
UID: NF:wdstptmgmt.IWdsTransportMulticastSessionPolicy.put_MultistreamStreamCount
title: IWdsTransportMulticastSessionPolicy::put_MultistreamStreamCount (wdstptmgmt.h)
description: Receives the maximum number of multicast streams per transmission used by the server.
old-location: wds\iwdstransportmulticastsessionpolicy_multistreamstreamcount.htm
tech.root: wds
ms.assetid: 34dd6dc0-3ff9-4dc3-9805-8fbfa972c4e1
ms.date: 12/05/2018
ms.keywords: IWdsTransportMulticastSessionPolicy interface [Windows Deployment Services],MultistreamStreamCount property, IWdsTransportMulticastSessionPolicy.MultistreamStreamCount, IWdsTransportMulticastSessionPolicy.put_MultistreamStreamCount, IWdsTransportMulticastSessionPolicy::MultistreamStreamCount, IWdsTransportMulticastSessionPolicy::get_MultistreamStreamCount, IWdsTransportMulticastSessionPolicy::put_MultistreamStreamCount, MultistreamStreamCount property [Windows Deployment Services], MultistreamStreamCount property [Windows Deployment Services],IWdsTransportMulticastSessionPolicy interface, put_MultistreamStreamCount, wds.iwdstransportmulticastsessionpolicy_multistreamstreamcount, wdstptmgmt/IWdsTransportMulticastSessionPolicy::MultistreamStreamCount, wdstptmgmt/IWdsTransportMulticastSessionPolicy::get_MultistreamStreamCount, wdstptmgmt/IWdsTransportMulticastSessionPolicy::put_MultistreamStreamCount
ms.topic: method
f1_keywords:
- wdstptmgmt/IWdsTransportMulticastSessionPolicy.MultistreamStreamCount
dev_langs:
- c++
req.header: wdstptmgmt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: Wdstptmgmt.tlb
req.lib: 
req.dll: Wdstptmgmt.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Wdstptmgmt.dll
api_name:
- IWdsTransportMulticastSessionPolicy.MultistreamStreamCount
- IWdsTransportMulticastSessionPolicy.get_MultistreamStreamCount
- IWdsTransportMulticastSessionPolicy.put_MultistreamStreamCount
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWdsTransportMulticastSessionPolicy::put_MultistreamStreamCount


## -description


Receives  the maximum number of multicast streams per transmission used by the server. If the server is configured to handle slow clients using the multistream method, the server detects clients that slow transmission below this maximum and moves them to lower-speed streams of the same multicast transmission.   The server cannot move legacy clients that do not support the multistream handling option, and in this case, the server disconnects the client or instructs the client to fallback depending upon the <a href="https://docs.microsoft.com/windows/desktop/api/wdstptmgmt/nf-wdstptmgmt-iwdstransportmulticastsessionpolicy-get_slowclientfallback">SlowClientFallback</a> property.

This property can be used to get or set the maximum stream count regardless of which method the server is using to handle  slow clients.

This property is read/write.


## -parameters


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wdstptmgmt/nn-wdstptmgmt-iwdstransportmulticastsessionpolicy">IWdsTransportMulticastSessionPolicy</a>
 

 

