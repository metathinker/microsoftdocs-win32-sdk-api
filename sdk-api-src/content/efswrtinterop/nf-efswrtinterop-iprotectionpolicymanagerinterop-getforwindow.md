---
UID: NF:efswrtinterop.IProtectionPolicyManagerInterop.GetForWindow
title: IProtectionPolicyManagerInterop::GetForWindow (efswrtinterop.h)
description: Returns the protection policy manager object associated with the current app window.
helpviewer_keywords: ["EDP.iprotectionpolicymanager_getforwindow","GetForWindow","GetForWindow method","GetForWindow method","IProtectionPolicyManagerInterop interface","IProtectionPolicyManagerInterop interface","GetForWindow method","IProtectionPolicyManagerInterop.GetForWindow","IProtectionPolicyManagerInterop::GetForWindow","efswrtinterop/IProtectionPolicyManagerInterop::GetForWindow"]
old-location: edp\iprotectionpolicymanager_getforwindow.htm
tech.root: EDP
ms.assetid: 638316E0-8D5C-4966-A44F-8F31ECBE83EB
ms.date: 12/05/2018
ms.keywords: EDP.iprotectionpolicymanager_getforwindow, GetForWindow, GetForWindow method, GetForWindow method,IProtectionPolicyManagerInterop interface, IProtectionPolicyManagerInterop interface,GetForWindow method, IProtectionPolicyManagerInterop.GetForWindow, IProtectionPolicyManagerInterop::GetForWindow, efswrtinterop/IProtectionPolicyManagerInterop::GetForWindow
req.header: efswrtinterop.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Efswrtinterop.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Efswrt.dll
req.irql: 
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
f1_keywords:
 - IProtectionPolicyManagerInterop::GetForWindow
 - efswrtinterop/IProtectionPolicyManagerInterop::GetForWindow
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - efswrt.dll
api_name:
 - IProtectionPolicyManagerInterop.GetForWindow
---

# IProtectionPolicyManagerInterop::GetForWindow


## -description

Returns the **[ProtectionPolicyManager](
 /uwp/api/windows.security.enterprisedata.protectionpolicymanager)**
object associated with the given window.

<div class="alert"><b>Note</b>  Windows Information Protection (WIP) policy can be applied on Windows 10, version 1607.</div>

## -parameters

### -param appWindow [in]

Type: **[HWND](/windows/win32/winprog/windows-data-types)**

The window to get the **ProtectionPolicyManager** for.

### -param riid [iid_is] [in, retval]

Type: **REFIID**

Must refer to the [interface identifier (IID)](
/openspecs/windows_protocols/ms-oaut/5583e1b8-454c-4147-9f56-f72416a15bee#gt_76ad3105-3f05-479d-a40c-c9c8fa2ebd83) 
for the interface **IProtectionPolicyManager**, which is implemented by
**ProtectionPolicyManager**.

This IID can be found in the [Microsoft Interface Definition Language (MIDL)](/windows/win32/midl/midl-start-page)
file for the **Windows.Security.EnterpriseData** namespace. For convenience, it is repeated below:

```
D5703E18-A08D-47E6-A240-9934D7165EB5
```

### -param result

Type: **void\*\***

The address of a pointer to **IProtectionPolicyManager**. On successful return from this method,
the pointer will be set to the protection policy manager object for the given window.

## -returns

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.

## -see-also

<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/efswrtinterop/nn-efswrtinterop-iprotectionpolicymanagerinterop">IProtectionPolicyManagerInterop</a>

