---
UID: NE:webservices.__unnamed_enum_104
title: WS_METADATA_PROPERTY_ID (webservices.h)
description: Each metadata property is of type WS_METADATA_PROPERTY, is identified by an ID, and has an associated value. If a property is not specified when the metadata is created, then its default value is used.
old-location: wsw\ws_metadata_property_id.htm
tech.root: wsw
ms.assetid: d3baa961-4701-4f2f-9263-5ac0266f6056
ms.date: 12/05/2018
ms.keywords: WS_METADATA_PROPERTY_HEAP_PROPERTIES, WS_METADATA_PROPERTY_HEAP_REQUESTED_SIZE, WS_METADATA_PROPERTY_HOST_NAMES, WS_METADATA_PROPERTY_ID, WS_METADATA_PROPERTY_ID enumeration [Web Services for Windows], WS_METADATA_PROPERTY_MAX_DOCUMENTS, WS_METADATA_PROPERTY_POLICY_PROPERTIES, WS_METADATA_PROPERTY_STATE, WS_METADATA_PROPERTY_VERIFY_HOST_NAMES, webservices/WS_METADATA_PROPERTY_HEAP_PROPERTIES, webservices/WS_METADATA_PROPERTY_HEAP_REQUESTED_SIZE, webservices/WS_METADATA_PROPERTY_HOST_NAMES, webservices/WS_METADATA_PROPERTY_ID, webservices/WS_METADATA_PROPERTY_MAX_DOCUMENTS, webservices/WS_METADATA_PROPERTY_POLICY_PROPERTIES, webservices/WS_METADATA_PROPERTY_STATE, webservices/WS_METADATA_PROPERTY_VERIFY_HOST_NAMES, wsw.ws_metadata_property_id
ms.topic: enum
f1_keywords:
- webservices/WS_METADATA_PROPERTY_ID
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- HeaderDef
api_location:
- WebServices.h
api_name:
- WS_METADATA_PROPERTY_ID
targetos: Windows
req.typenames: WS_METADATA_PROPERTY_ID
req.redist: 
ms.custom: 19H1
---

# WS_METADATA_PROPERTY_ID enumeration


## -description


Each metadata property is of type <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_metadata_property">WS_METADATA_PROPERTY</a>, is identified by an ID, and has an associated value.  If a property is not specified when the metadata is created,
                then its default value is used.
            


## -enum-fields




### -field WS_METADATA_PROPERTY_STATE

This property is used with <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wsgetmetadataproperty">WsGetMetadataProperty</a>.
                

The accompanying <b>value</b> member of the <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_metadata_property">WS_METADATA_PROPERTY</a> structure contains  the current <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ne-webservices-ws_metadata_state">WS_METADATA_STATE</a> of the metadata object.
                


### -field WS_METADATA_PROPERTY_HEAP_PROPERTIES

This property is used with <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wscreatemetadata">WsCreateMetadata</a> to specify
                    properties of the <a href="https://docs.microsoft.com/windows/desktop/wsw/ws-heap">WS_HEAP</a> object used by the metadata
                    object to store information about the metadata that was read.
                

The accompanying <b>value</b> member of the <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_metadata_property">WS_METADATA_PROPERTY</a> structure contains   a <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_heap_properties">WS_HEAP_PROPERTIES</a> structure.
                

The following heap properties may be specified:
                

<ul>
<li>
<a href="https://docs.microsoft.com/windows/desktop/api/webservices/ne-webservices-ws_heap_property_id">WS_HEAP_PROPERTY_MAX_SIZE</a>.  If not specified, the
                    default value used is 256k bytes.
                    </li>
<li>
<a href="https://docs.microsoft.com/windows/desktop/api/webservices/ne-webservices-ws_heap_property_id">WS_HEAP_PROPERTY_TRIM_SIZE</a>.  If not specified, the
                    default value used is 32k bytes.
                </li>
</ul>

### -field WS_METADATA_PROPERTY_POLICY_PROPERTIES

This property is used with <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wscreatemetadata">WsCreateMetadata</a> to specify
                    properties of the <a href="https://docs.microsoft.com/windows/desktop/wsw/ws-policy">WS_POLICY</a> objects that are associated
                    with the metadata object.
                

The accompanying <b>value</b> member of the <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_metadata_property">WS_METADATA_PROPERTY</a> structure contains   a <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_policy_properties">WS_POLICY_PROPERTIES</a>  structure that specifies the
                    set of policy properties.

See <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ne-webservices-ws_policy_property_id">WS_POLICY_PROPERTY_ID</a> for more information on the
                    set of properties that may be specified here.
                


### -field WS_METADATA_PROPERTY_HEAP_REQUESTED_SIZE

This property is used with <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wsgetmetadataproperty">WsGetMetadataProperty</a>.
                

The accompanying <b>value</b> member of the <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_metadata_property">WS_METADATA_PROPERTY</a> is a <b>SIZE_T</b> specifying the number of bytes allocated from the heap associated with the
                    metadata object.


### -field WS_METADATA_PROPERTY_MAX_DOCUMENTS

This property is used with <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wscreatemetadata">WsCreateMetadata</a>.
                

The accompanying <b>value</b> member of the <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_metadata_property">WS_METADATA_PROPERTY</a> is a <b>ULONG</b> specifying  the maximum number of documents that may be added to
                    the metadata object using <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wsreadmetadata">WsReadMetadata</a>.  
                

The default value is 32.
                


### -field WS_METADATA_PROPERTY_HOST_NAMES

This property is used with <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wscreatemetadata">WsCreateMetadata</a>.
                

The accompanying <b>value</b> member of the <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_metadata_property">WS_METADATA_PROPERTY</a> is a <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_host_names">WS_HOST_NAMES</a> structure.
                

This property may only be specified if <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ne-webservices-ws_metadata_property_id">WS_METADATA_PROPERTY_VERIFY_HOST_NAMES</a> is <b>TRUE</b>.
                

See <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wsgetmissingmetadatadocumentaddress">WsGetMissingMetadataDocumentAddress</a> for more information
                    on verifying host names.
                

If the property is not specified, then the list of host names is empty.
                


### -field WS_METADATA_PROPERTY_VERIFY_HOST_NAMES

This property is used with <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wscreatemetadata">WsCreateMetadata</a>.
                

The accompanying <b>value</b> member of the <a href="https://docs.microsoft.com/windows/desktop/api/webservices/ns-webservices-ws_metadata_property">WS_METADATA_PROPERTY</a> is a <b>BOOL</b> that specifies whether or not host names should be verified.
                

See <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wsgetmissingmetadatadocumentaddress">WsGetMissingMetadataDocumentAddress</a> for more information
                    on verifying host names.
                

The default value is <b>TRUE</b>.
                

Setting this value to <b>FALSE</b> may cause an application to use
                    an address returned from <a href="https://docs.microsoft.com/windows/desktop/api/webservices/nf-webservices-wsgetmissingmetadatadocumentaddress">WsGetMissingMetadataDocumentAddress</a>that is from a host that it is not willing to accept metadata from.
                

