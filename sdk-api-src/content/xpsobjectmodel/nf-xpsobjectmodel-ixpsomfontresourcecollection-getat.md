---
UID: NF:xpsobjectmodel.IXpsOMFontResourceCollection.GetAt
title: IXpsOMFontResourceCollection::GetAt (xpsobjectmodel.h)
description: Gets an IXpsOMFontResource interface pointer from a specified location in the collection.
helpviewer_keywords: ["GetAt","GetAt method [XPS Documents and Packaging]","GetAt method [XPS Documents and Packaging]","IXpsOMFontResourceCollection interface","IXpsOMFontResourceCollection interface [XPS Documents and Packaging]","GetAt method","IXpsOMFontResourceCollection.GetAt","IXpsOMFontResourceCollection::GetAt","xps.ixpsomfontresourcecollection_getat","xpsobjectmodel/IXpsOMFontResourceCollection::GetAt"]
old-location: xps\ixpsomfontresourcecollection_getat.htm
tech.root: xps
ms.assetid: c97409fd-3210-4177-8b8e-46a725d17425
ms.date: 12/05/2018
ms.keywords: GetAt, GetAt method [XPS Documents and Packaging], GetAt method [XPS Documents and Packaging],IXpsOMFontResourceCollection interface, IXpsOMFontResourceCollection interface [XPS Documents and Packaging],GetAt method, IXpsOMFontResourceCollection.GetAt, IXpsOMFontResourceCollection::GetAt, xps.ixpsomfontresourcecollection_getat, xpsobjectmodel/IXpsOMFontResourceCollection::GetAt
req.header: xpsobjectmodel.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: XpsObjectModel.idl
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
 - IXpsOMFontResourceCollection::GetAt
 - xpsobjectmodel/IXpsOMFontResourceCollection::GetAt
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - xpsobjectmodel.h
api_name:
 - IXpsOMFontResourceCollection.GetAt
---

# IXpsOMFontResourceCollection::GetAt


## -description

Gets an <a href="/windows/desktop/api/xpsobjectmodel/nn-xpsobjectmodel-ixpsomfontresource">IXpsOMFontResource</a> interface pointer from a specified location in the collection.

## -parameters

### -param index [in]

The zero-based index of the <a href="/windows/desktop/api/xpsobjectmodel/nn-xpsobjectmodel-ixpsomfontresource">IXpsOMFontResource</a> interface pointer to be obtained.

### -param value [out, retval]

The <a href="/windows/desktop/api/xpsobjectmodel/nn-xpsobjectmodel-ixpsomfontresource">IXpsOMFontResource</a> interface pointer at the location specified by <i>index</i>.

## -returns

If the method succeeds, it returns S_OK; otherwise, it returns an <b>HRESULT</b> error code.

## -remarks

For more information about the collection methods, see  <a href="/previous-versions/windows/desktop/dd372931(v=vs.85)">Working with XPS OM Collection Interfaces</a>.

## -see-also

<a href="/windows/desktop/api/xpsobjectmodel/nn-xpsobjectmodel-ixpsomfontresource">IXpsOMFontResource</a>



<a href="/windows/desktop/api/xpsobjectmodel/nn-xpsobjectmodel-ixpsomfontresourcecollection">IXpsOMFontResourceCollection</a>



<a href="/previous-versions/windows/desktop/dd372931(v=vs.85)">Working with XPS OM Collection Interfaces</a>



<a href="https://www.microsoft.com/download/details.aspx?id=11816">XML Paper Specification</a>