---
UID: NF:setupapi.SetupGetFileCompressionInfoExA
title: SetupGetFileCompressionInfoExA function (setupapi.h)
description: The SetupGetFileCompressionInfoEx function examines a potentially compressed file and gets the type of compression, the file's full path (including file name), the compressed size, and the size of the uncompressed target file.
old-location: setup\setupgetfilecompressioninfoex.htm
tech.root: SetupApi
ms.assetid: e6f01e02-ea39-4b25-bcc0-2aee941c7834
ms.date: 12/05/2018
ms.keywords: SetupGetFileCompressionInfoEx, SetupGetFileCompressionInfoEx function [Setup API], SetupGetFileCompressionInfoExA, SetupGetFileCompressionInfoExW, _setupapi_setupgetfilecompressioninfoex, setup.setupgetfilecompressioninfoex, setupapi/SetupGetFileCompressionInfoEx, setupapi/SetupGetFileCompressionInfoExA, setupapi/SetupGetFileCompressionInfoExW
ms.topic: function
f1_keywords:
- setupapi/SetupGetFileCompressionInfoEx
dev_langs:
- c++
req.header: setupapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: SetupGetFileCompressionInfoExW (Unicode) and SetupGetFileCompressionInfoExA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Setupapi.lib
req.dll: Setupapi.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Setupapi.dll
api_name:
- SetupGetFileCompressionInfoEx
- SetupGetFileCompressionInfoExA
- SetupGetFileCompressionInfoExW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# SetupGetFileCompressionInfoExA function


## -description


<p class="CCE_Message">[This function is available for use in the operating systems indicated in the Requirements section. It may be altered or unavailable in subsequent versions.   SetupAPI should no longer be used for installing applications. Instead, use the Windows Installer for developing application installers. SetupAPI continues to be used for installing device drivers.]

The 
<b>SetupGetFileCompressionInfoEx</b> function examines a potentially compressed file and gets the type of compression, the file's full path (including file name), the compressed size, and the size of the uncompressed target file. The caller of the function passes in the name of the file to be examined and pointers to locations for the buffer and buffer size to receive the returned file name and path.

To determine the size of the buffer for the returned path and file name, you can call 
<b>SetupGetFileCompressionInfoEx</b> with <i>ActualSourceFileNameBuffer</i> specified <b>Null</b> and <i>ActualSourceFileNameLen</i> containing 0. The function succeeds and on return fills in <i>RequiredBufferLen</i>.


## -parameters




### -param SourceFileName [in]

File name of the potentially compressed file to be examined. If the file is not found on the source media exactly as named, Setup searches for up to two alternate names. For example; if Setup does not find F:\x86\cmd.exe, it searches for F:\mpis\cmd.ex_ and if that name is not found, it searches for F:\x86\cmd.ex$.


### -param ActualSourceFileNameBuffer [in, out]

Pointer to a  buffer that receives the actual file name and path if this parameter is not <b>NULL</b>. This is valid only if the function returns NO_ERROR.


### -param ActualSourceFileNameBufferLen [in, out]

Size of the buffer specified by <i>ActualSourceFileNameBuffer</i>, in characters. You would typically use a buffer size of MAX_PATH. If <i>ActualSourceFileNameLen</i> is too small, the function fails with ERROR_INSUFFICIENT_BUFFER. <i>ActualSourceFileNameLen</i> must contain zero if <i>ActualSourceFileNameBuffer</i> is <b>NULL</b>.


### -param RequiredBufferLen [out]

Size of the file name and full path including the terminating <b>NULL</b>, if this parameter is not <b>NULL</b>. If <i>ActualSourceFileNameBuffer</i> is <b>NULL</b> and <i>ActualSourceFileNameLen</i> is zero, the function succeeds but fills in <i>RequiredBufferLen</i>. This parameter is valid only if the function returns NO_ERROR or ERROR_INSUFFICIENT_BUFFER.


### -param SourceFileSize [out]

Pointer to a variable in which this function returns the size of the file in its current form, which is the current size of the file named by <i>ActualSourceFileNameBuffer</i>. The size is determined by examining the source file; it is not retrieved from an INF file. The source file size is valid only if the function returns NO_ERROR or ERROR_INSUFFICIENT_BUFFER.


### -param TargetFileSize [out]

Pointer to a variable in which this function returns the size that the file will occupy when it is uncompressed or copied. If the file is not compressed, this value will be the same as <i>SourceFileSize</i>. The size is determined by examining the file; it is not retrieved from an INF file. The target file size is valid only if the function returns NO_ERROR or ERROR_INSUFFICIENT_BUFFER.


### -param CompressionType [out]

Pointer to a variable in which this function returns a value indicating the type of compression used on <i>ActualSourceFileName</i>. The compression type is valid only if the function returns NO_ERROR or ERROR_INSUFFICIENT_BUFFER. This parameter value can be one of the following flags. 







#### FILE_COMPRESSION_NONE

The source file is not compressed with a recognized compression algorithm.



#### FILE_COMPRESSION_WINLZA

The source file is compressed with LZ compression.



#### FILE_COMPRESSION_MSZIP

The source file is compressed with MSZIP compression.


## -returns



If the function succeeds, the return value is <b>TRUE</b> (nonzero).

If the function fails, the return value is <b>FALSE</b> (zero). The function can also return one of the following  <a href="https://docs.microsoft.com/windows/desktop/Debug/system-error-codes">system error codes</a>.

To get extended error information, call 
<a href="https://docs.microsoft.com/windows/desktop/api/errhandlingapi/nf-errhandlingapi-getlasterror">GetLastError</a>.




## -remarks



Because 
<b>SetupGetFileCompressionInfoEx</b> determines the compression by examining the physical file, your setup application should ensure that the file is present before calling 
<b>SetupGetFileCompressionInfoEx</b>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/SetupApi/functions">Functions</a>



<a href="https://docs.microsoft.com/windows/desktop/SetupApi/overview">Overview</a>



<a href="https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdecompressorcopyfilea">SetupDecompressOrCopyFile</a>
 

 

