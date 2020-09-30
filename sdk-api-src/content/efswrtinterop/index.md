---
UID: NA:efswrtinterop
title: Efswrtinterop.h header
ms.assetid: 7abe7af0-89b1-33bb-a90b-5f41c2980004
ms.date: 01/11/2019
ms.keywords: 
ms.topic: conceptual
tech.root: edp
archived: true
f1_keywords:
 - efswrtinterop
 - efswrtinterop/efswrtinterop
---

# Efswrtinterop.h header

Gives desktop applications access to some static methods of
**[Windows.Security.EnterpriseData.ProtectionPolicyManager](
 /uwp/api/windows.security.enterprisedata.protectionpolicymanager)**
that are otherwise available only to Universal Windows Platform apps.

## -description

This header is used by Windows Information Protection (WIP). For more information, see:

- [Windows Information Protection (WIP)](../_edp/index.md)

## -remarks

All interfaces in this header file are implemented by **ProtectionPolicyManager**'s [activation factory](
../activation/nn-activation-iactivationfactory).
To get a object of an interface in this header, get a reference to the activation factory and then call
[IUnknown::QueryInterface](../unknwn/nf-unknwn-iunknown-queryinterface%28refiid_void%29)
on that reference:

```cppwinrt
using winrt::Windows::Security::EnterpriseData::ProtectionPolicyManager;

auto managerFactory = winrt::get_activation_factory<ProtectionPolicyManager>();

winrt::com_ptr<IProtectionPolicyManagerInterop> managerInterop{ managerFactory.as<IProtectionPolicyManagerInterop>() };
// You can now call methods of IProtectionPolicyManagerInterop on `managerInterop`.

winrt::com_ptr<IProtectionPolicyManagerInterop2> managerInterop2{ managerFactory.as<IProtectionPolicyManagerInterop2>() };
// You can now call methods of IProtectionPolicyManagerInterop2 on `managerInterop2`.
```

