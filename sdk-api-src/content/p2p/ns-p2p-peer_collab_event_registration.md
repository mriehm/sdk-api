---
UID: NS:p2p.peer_collab_event_registration_tag
title: PEER_COLLAB_EVENT_REGISTRATION (p2p.h)
description: The PEER_COLLAB_EVENT_REGISTRATION structure contains the data used by a peer to register for specific peer collaboration network events.
old-location: p2p\peer_collab_event_registration.htm
tech.root: P2PSdk
ms.assetid: dfc55346-99ef-441e-ba49-e7463581ebbb
ms.date: 12/05/2018
ms.keywords: '*PPEER_COLLAB_EVENT_REGISTRATION, PCPEER_COLLAB_EVENT_REGISTRATION, PCPEER_COLLAB_EVENT_REGISTRATION structure pointer [Peer Networking], PEER_COLLAB_EVENT_REGISTRATION, PEER_COLLAB_EVENT_REGISTRATION structure [Peer Networking], PPEER_COLLAB_EVENT_REGISTRATION, PPEER_COLLAB_EVENT_REGISTRATION structure pointer [Peer Networking], p2p.peer_collab_event_registration, p2p/PCPEER_COLLAB_EVENT_REGISTRATION, p2p/PEER_COLLAB_EVENT_REGISTRATION, p2p/PPEER_COLLAB_EVENT_REGISTRATION'
ms.topic: struct
f1_keywords:
- p2p/PEER_COLLAB_EVENT_REGISTRATION
dev_langs:
- c++
req.header: p2p.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: None supported
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
- HeaderDef
api_location:
- P2P.h
api_name:
- PEER_COLLAB_EVENT_REGISTRATION
targetos: Windows
req.typenames: PEER_COLLAB_EVENT_REGISTRATION, *PPEER_COLLAB_EVENT_REGISTRATION
req.redist: 
ms.custom: 19H1
---

# PEER_COLLAB_EVENT_REGISTRATION structure


## -description


The <b>PEER_COLLAB_EVENT_REGISTRATION</b> structure contains the data used by a peer to register for specific peer collaboration network events.


## -struct-fields




### -field eventType


<a href="https://docs.microsoft.com/windows/desktop/api/p2p/ne-p2p-peer_collab_event_type">PEER_COLLAB_EVENT_TYPE</a> enumeration value that specifies the type of peer collaboration network event for which to register.


### -field pInstance

GUID value that uniquely identifies the application or object  that registers for the specific event.

This parameter is valid only for PEER_EVENT_ENDPOINT_APPLICATION_CHANGED, PEER_EVENT_ENDPOINT_OBJECT_CHANGED, PEER_EVENT_MY_APPLICATION_CHANGED, and PEER_EVENT_MY_OBJECT_CHANGED. This GUID represents the application ID for application-specific events, and the object ID for object-specific events.  

When <b></b>this member is set, notification will be sent only for the specific application or object.


### -field pInstance.unique

 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/p2p/ne-p2p-peer_collab_event_type">PEER_COLLAB_EVENT_TYPE</a>



<a href="https://docs.microsoft.com/windows/desktop/P2PSdk/collaboration-api-structures">Peer Collaboration API Structures</a>
 

 

