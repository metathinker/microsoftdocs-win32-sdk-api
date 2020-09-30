---
UID: NN:efswrtinterop.IProtectionPolicyManagerInterop
title: IProtectionPolicyManagerInterop (efswrtinterop.h)
description: Manages enterprise protection policy on protected content.
helpviewer_keywords: ["EDP.iprotectionpolicymanagerinterop","IProtectionPolicyManagerInterop","IProtectionPolicyManagerInterop interface","IProtectionPolicyManagerInterop interface","described","efswrtinterop/IProtectionPolicyManagerInterop interface"]
old-location: edp\iprotectionpolicymanagerinterop.htm
tech.root: EDP
ms.assetid: AFA7F918-8730-40A2-871E-9356391B47F8
ms.date: 12/05/2018
ms.keywords: EDP.iprotectionpolicymanagerinterop, IProtectionPolicyManagerInterop, IProtectionPolicyManagerInterop interface, IProtectionPolicyManagerInterop interface,described, efswrtinterop/IProtectionPolicyManagerInterop interface
req.header: efswrtinterop.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
f1_keywords:
 - IProtectionPolicyManagerInterop
 - efswrtinterop/IProtectionPolicyManagerInterop
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - efswrtinterop.h
api_name:
 - IProtectionPolicyManagerInterop
---

# IProtectionPolicyManagerInterop interface

## -description

Gives desktop applications access to some static methods of
**[Windows.Security.EnterpriseData.ProtectionPolicyManager](
 /uwp/api/windows.security.enterprisedata.protectionpolicymanager)**
that are otherwise available only to Universal Windows Platform apps.

<div class="alert"><b>Note</b>  Windows Information Protection (WIP) policy can be applied on Windows 10, version 1607.</div>

## -inheritance

The **IProtectionPolicyManagerInterop** interface inherits from the **[IInspectable](../inspectable/nn-inspectable-iinspectable)** interface.

## -remarks

This interface is implemented by **ProtectionPolicyManager**'s [activation factory](../activation/nn-activation-iactivationfactory).
To get an object of this interface, get a reference to the activation factory and then call
[IUnknown::QueryInterface](../unknwn/nf-unknwn-iunknown-queryinterface%28refiid_void%29)
on that reference:

```cppwinrt
using winrt::Windows::Security::EnterpriseData::ProtectionPolicyManager;

auto managerFactory = winrt::get_activation_factory<ProtectionPolicyManager>();
winrt::com_ptr<IProtectionPolicyManagerInterop> managerInterop{ managerFactory.as<IProtectionPolicyManagerInterop>() };
// You can now call methods of IProtectionPolicyManagerInterop on `managerInterop`.
```

<!--
## -members

The <b>IProtectionPolicyManagerInterop</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/efswrtinterop/nf-efswrtinterop-iprotectionpolicymanagerinterop-getforwindow">IProtectionPolicyManagerInterop::GetForWindow</a>
</td>
<td align="left" width="63%">
Returns the protection policy manager object associated with the current app window.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/efswrtinterop/nf-efswrtinterop-iprotectionpolicymanagerinterop-requestaccessforwindowasync">IProtectionPolicyManagerInterop::RequestAccessForWindowAsync</a>
</td>
<td align="left" width="63%">
Request access to enterprise protected content for an identity.

</td>
</tr>
</table>

-->
