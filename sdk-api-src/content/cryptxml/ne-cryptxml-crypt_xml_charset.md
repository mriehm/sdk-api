---
UID: NE:cryptxml.__unnamed_enum_0
title: CRYPT_XML_CHARSET (cryptxml.h)
description: Used to specify the character set used in the XML.
old-location: security\crypt_xml_charset.htm
tech.root: SecCrypto
ms.assetid: 3f115ac1-a8ed-4151-b3f3-7ddb695802a0
ms.date: 12/05/2018
ms.keywords: CRYPT_XML_CHARSET, CRYPT_XML_CHARSET enumeration [Security], CRYPT_XML_CHARSET_AUTO, CRYPT_XML_CHARSET_UTF16BE, CRYPT_XML_CHARSET_UTF16LE, CRYPT_XML_CHARSET_UTF8, cryptxml/CRYPT_XML_CHARSET, cryptxml/CRYPT_XML_CHARSET_AUTO, cryptxml/CRYPT_XML_CHARSET_UTF16BE, cryptxml/CRYPT_XML_CHARSET_UTF16LE, cryptxml/CRYPT_XML_CHARSET_UTF8, security.crypt_xml_charset
ms.topic: enum
f1_keywords:
- cryptxml/CRYPT_XML_CHARSET
dev_langs:
- c++
req.header: cryptxml.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
- Cryptxml.h
api_name:
- CRYPT_XML_CHARSET
targetos: Windows
req.typenames: CRYPT_XML_CHARSET
req.redist: 
ms.custom: 19H1
---

# CRYPT_XML_CHARSET enumeration


## -description


The <b>CRYPT_XML_CHARSET</b> enumeration is used to specify the character set used in the XML.


## -enum-fields




### -field CRYPT_XML_CHARSET_AUTO

This value is only supported in the <a href="https://docs.microsoft.com/windows/desktop/api/cryptxml/nf-cryptxml-cryptxmlopentodecode">CryptXmlOpenToDecode</a> function. The encoded XML character set is determined by the parser and is based on the XML declaration or the best guess on the characters.


### -field CRYPT_XML_CHARSET_UTF8

Specifies the UTF-8 character set.


### -field CRYPT_XML_CHARSET_UTF16LE

Specifies the UTF-16 little-endian character set.


### -field CRYPT_XML_CHARSET_UTF16BE

Specifies the UTF-16 big-endian character set.

