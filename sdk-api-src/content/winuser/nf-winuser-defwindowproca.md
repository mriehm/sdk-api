---
UID: NF:winuser.DefWindowProcA
title: DefWindowProcA function (winuser.h)
description: Calls the default window procedure to provide default processing for any window messages that an application does not process.
old-location: winmsg\defwindowproc.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\windowprocedures\windowprocedurereference\windowprocedurefunctions\defwindowproc.htm
ms.date: 12/05/2018
ms.keywords: DefWindowProc, DefWindowProc function [Windows and Messages], DefWindowProcA, DefWindowProcW, _win32_DefWindowProc, _win32_defwindowproc_cpp, winmsg.defwindowproc, winui._win32_defwindowproc, winuser/DefWindowProc, winuser/DefWindowProcA, winuser/DefWindowProcW
ms.topic: function
f1_keywords:
- winuser/DefWindowProc
dev_langs:
- c++
req.header: winuser.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: DefWindowProcW (Unicode) and DefWindowProcA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- User32.dll
- API-MS-Win-NTUser-IE-Window-l1-1-0.dll
- ie_shims.dll
- API-MS-Win-RTCore-NTUser-Window-l1-1-0.dll
- minuser.dll
- Ext-MS-Win-NTUser-Window-l1-1-0.dll
- Ext-MS-Win-NTUser-Window-l1-1-1.dll
- Ext-MS-Win-NTUser-Window-l1-1-2.dll
- Ext-MS-Win-RTCore-NTUser-Window-Ext-l1-1-0.dll
- ext-ms-win-ntuser-window-l1-1-3.dll
- Ext-MS-Win-NTUser-Window-L1-1-4.dll
api_name:
- DefWindowProc
- DefWindowProcA
- DefWindowProcW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# DefWindowProcA function


## -description


Calls the default window procedure to provide default processing for any window messages that an application does not process. This function ensures that every message is processed. <b>DefWindowProc</b> is called with the same parameters received by the window procedure. 


## -parameters




### -param hWnd [in]

Type: <b>HWND</b>

A handle to the window procedure that received the message. 


### -param Msg [in]

Type: <b>UINT</b>

The message. 


### -param wParam [in]

Type: <b>WPARAM</b>

Additional message information. The content of this parameter depends on the value of the <i>Msg</i> parameter. 


### -param lParam [in]

Type: <b>LPARAM</b>

Additional message information. The content of this parameter depends on the value of the <i>Msg</i> parameter. 


## -returns



Type: <strong>Type: <b>LRESULT</b>
</strong>

The return value is the result of the message processing and depends on the message. 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/winuser/nf-winuser-callwindowproca">CallWindowProc</a>



<b>Conceptual</b>



<a href="https://docs.microsoft.com/windows/desktop/api/winuser/nf-winuser-defdlgprocw">DefDlgProc</a>



<b>Reference</b>



<a href="https://docs.microsoft.com/windows/desktop/winmsg/window-procedures">Window Procedures</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/legacy/ms633573(v=vs.85)">WindowProc</a>
 

 

