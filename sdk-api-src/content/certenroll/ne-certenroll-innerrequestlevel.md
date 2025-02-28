---
UID: NE:certenroll.InnerRequestLevel
title: InnerRequestLevel (certenroll.h)
description: Specifies the containment level of a certificate request within a PKCS
old-location: security\innerrequestlevel_enum.htm
tech.root: seccertenroll
ms.assetid: 57b16024-5347-4218-90a7-d85e403aacf0
ms.date: 12/05/2018
ms.keywords: InnerRequestLevel, InnerRequestLevel enumeration [Security], LevelInnermost, LevelNext, certenroll/InnerRequestLevel, certenroll/LevelInnermost, certenroll/LevelNext, security.innerrequestlevel_enum
ms.topic: enum
f1_keywords:
- certenroll/InnerRequestLevel
dev_langs:
- c++
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
- CertEnroll.h
api_name:
- InnerRequestLevel
targetos: Windows
req.typenames: InnerRequestLevel
req.redist: 
ms.custom: 19H1
---

# InnerRequestLevel enumeration


## -description


The <b>InnerRequestLevel</b> enumeration type specifies the containment level of a <a href="https://docs.microsoft.com/windows/desktop/SecGloss/c-gly">certificate request</a> within a PKCS #7 or <a href="https://docs.microsoft.com/windows/desktop/SecGloss/c-gly">Certificate Management over CMS</a> (CMC) request. This enumeration is used by the <a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nf-certenroll-ix509certificaterequest-getinnerrequest">GetInnerRequest</a> method on the <a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nn-certenroll-ix509certificaterequest">IX509CertificateRequest</a> interface and inherited by the <a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nn-certenroll-ix509certificaterequestpkcs7">IX509CertificateRequestPkcs7</a> and <a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nn-certenroll-ix509certificaterequestcmc">IX509CertificateRequestCmc</a> interfaces. You can use the enumeration values to retrieve the innermost nested certificate or to iterate through all of the nesting levels.


## -enum-fields




### -field LevelInnermost

Use to retrieve the most deeply nested request.


### -field LevelNext

Use to retrieve the request at the next nesting level.


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/SecCertEnroll/certenroll-enumerations">CertEnroll Enumerations</a>



<a href="https://docs.microsoft.com/windows/desktop/SecCertEnroll/certenroll-interfaces">CertEnroll Interfaces</a>



<a href="https://docs.microsoft.com/windows/desktop/api/certenroll/nf-certenroll-ix509certificaterequest-getinnerrequest">GetInnerRequest</a>
 

 

