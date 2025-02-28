---
UID: NS:mfapi._MFCameraExtrinsics
title: MFCameraExtrinsics (mfapi.h)
description: Describes the location of a camera relative to other cameras or an established external reference.
old-location: mf\mfcameraextrinsics.htm
tech.root: medfound
ms.assetid: F29615EE-0B2C-4066-8A6B-67457D46028C
ms.date: 12/05/2018
ms.keywords: MFCameraExtrinsics, MFCameraExtrinsics structure [Media Foundation], PMFCameraExtrinsics, PMFCameraExtrinsics structure pointer [Media Foundation], mf.mfcameraextrinsics, mfapi/MFCameraExtrinsics, mfapi/PMFCameraExtrinsics
ms.topic: struct
f1_keywords:
- mfapi/MFCameraExtrinsics
dev_langs:
- c++
req.header: mfapi.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- HeaderDef
api_location:
- mfapi.h
api_name:
- MFCameraExtrinsics
targetos: Windows
req.typenames: MFCameraExtrinsics
req.redist: 
ms.custom: 19H1
---

# MFCameraExtrinsics structure


## -description


Describes the location of a camera relative to other cameras or an established external reference.  


## -struct-fields




### -field TransformCount

The number of transforms in the <i>CalibratedTransforms</i> array.


### -field CalibratedTransforms

The array of transforms in the extrinsic data.


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/medfound/media-foundation-structures">Media Foundation Structures</a>
 

 

