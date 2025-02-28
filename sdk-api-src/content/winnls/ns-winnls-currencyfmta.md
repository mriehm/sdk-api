---
UID: NS:winnls._currencyfmtA
title: CURRENCYFMTA (winnls.h)
description: Contains information that defines the format of a currency string. The GetCurrencyFormat function uses this information to customize a currency string for a specified locale.
old-location: intl\currencyfmt.htm
tech.root: Intl
ms.assetid: 026ac9e0-1f5b-4a42-9c7b-07a127422994
ms.date: 12/05/2018
ms.keywords: '*LPCURRENCYFMTA, CURRENCYFMT, CURRENCYFMT structure [Internationalization for Windows Applications], CURRENCYFMTA, LPCURRENCYFMT, LPCURRENCYFMT structure pointer [Internationalization for Windows Applications], _win32_CURRENCYFMT_str, intl.currencyfmt, winnls/CURRENCYFMT, winnls/LPCURRENCYFMT'
ms.topic: struct
f1_keywords:
- winnls/CURRENCYFMT
dev_langs:
- c++
req.header: winnls.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
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
- Winnls.h
api_name:
- CURRENCYFMT
targetos: Windows
req.typenames: CURRENCYFMTA, *LPCURRENCYFMTA
req.redist: 
ms.custom: 19H1
---

# CURRENCYFMTA structure


## -description



Contains information that defines the format of a currency string. The <a href="https://docs.microsoft.com/windows/desktop/api/winnls/nf-winnls-getcurrencyformata">GetCurrencyFormat</a> function uses this information to customize a currency string for a specified locale.




## -struct-fields




### -field NumDigits

Number of fractional digits. This number is equivalent to <a href="https://docs.microsoft.com/windows/desktop/Intl/locale-icurrdigits">LOCALE_ICURRDIGITS</a>.


### -field LeadingZero

Value indicating if leading zeros should be used in decimal fields. This value is equivalent to <a href="https://docs.microsoft.com/windows/desktop/Intl/locale-ilzero">LOCALE_ILZERO</a>.


### -field Grouping

Number of digits in each group of numbers to the left of the decimal separator specified by <b>lpDecimalSep</b>. The most significant grouping digit indicates the number of digits in the least significant group immediately to the left of the decimal separator. Each subsequent grouping digit indicates the next significant group of digits to the left of the previous group. If the last value supplied is not 0, the remaining groups repeat the last group. Typical examples of settings for this member are: 0 to group digits as in 123456789.00; 3 to group digits as in 123,456,789.00; and 32 to group digits as in 12,34,56,789.00.

<div class="alert"><b>Note</b>   You can use settings other than the typical settings, but they will not show up in the regional and language settings portion of the Control Panel. Such settings are extremely uncommon and might have unexpected results.</div>
<div> </div>

### -field lpDecimalSep

Pointer to a null-terminated decimal separator string.


### -field lpThousandSep

Pointer to a null-terminated thousand separator string.


### -field NegativeOrder

Negative currency mode. This mode is equivalent to <a href="https://docs.microsoft.com/windows/desktop/Intl/locale-ineg-constants">LOCALE_INEGCURR</a>.


### -field PositiveOrder

Positive currency mode. This mode is equivalent to <a href="https://docs.microsoft.com/windows/desktop/Intl/locale-icurrency">LOCALE_ICURRENCY</a>.


### -field lpCurrencySymbol

Pointer to a null-terminated currency symbol string.


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/winnls/nf-winnls-getcurrencyformata">GetCurrencyFormat</a>



<a href="https://docs.microsoft.com/windows/desktop/Intl/national-language-support-structures">National Language Support Structures</a>
 

 

