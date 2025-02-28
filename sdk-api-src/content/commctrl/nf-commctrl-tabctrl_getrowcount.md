---
UID: NF:commctrl.TabCtrl_GetRowCount
title: TabCtrl_GetRowCount macro (commctrl.h)
description: Retrieves the current number of rows of tabs in a tab control. You can use this macro or send the TCM_GETROWCOUNT message explicitly.
old-location: controls\TabCtrl_GetRowCount.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\tab\macros\tabctrl_getrowcount.htm
ms.date: 12/05/2018
ms.keywords: TabCtrl_GetRowCount, TabCtrl_GetRowCount macro [Windows Controls], _win32_TabCtrl_GetRowCount, _win32_TabCtrl_GetRowCount_cpp, commctrl/TabCtrl_GetRowCount, controls.TabCtrl_GetRowCount, controls._win32_TabCtrl_GetRowCount
ms.topic: macro
f1_keywords:
- commctrl/TabCtrl_GetRowCount
dev_langs:
- c++
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
- Commctrl.h
api_name:
- TabCtrl_GetRowCount
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# TabCtrl_GetRowCount macro


## -description


Retrieves the current number of rows of tabs in a tab control. You can use this macro or send the <a href="https://docs.microsoft.com/windows/desktop/Controls/tcm-getrowcount">TCM_GETROWCOUNT</a> message explicitly. 


## -parameters




### -param hwnd

Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">HWND</a></b>

Handle to the tab control. 


## -remarks



Only tab controls that have the <a href="https://docs.microsoft.com/windows/desktop/Controls/tab-control-styles">TCS_MULTILINE</a> style can have multiple rows of tabs. 



