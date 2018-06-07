---
title: licensed attribute
description: The \ licensed\ attribute indicates that the coclass to which it applies is licensed, and must be instantiated using IClassFactory2.
ms.assetid: c4789ea2-8ff6-423e-8b69-22a7a5392854
keywords:
- licensed attribute MIDL
topic_type:
- apiref
api_name:
- licensed
api_type:
- NA
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# licensed attribute

The **\[licensed\]** attribute indicates that the [**coclass**](coclass.md) to which it applies is licensed, and must be instantiated using [**IClassFactory2**](c49c7612-3b1f-4535-baf3-8458b3f34f95).

``` syntax
[
    licensed
    [ , attribute-list ] 
]
coclass classname 
{
  coclass-definition
};
```

## Parameters

<dl> <dt>

*attribute-list* 
</dt> <dd>

Specifies zero or more attributes that apply to the [**coclass**](coclass.md) statement. Allowable **coclass** attributes are **\[**[**helpstring**](helpstring.md)**\]**, **\[**[**helpcontext**](helpcontext.md)**\]**, **\[licensed\]**, **\[**[**version**](version.md)**\]**, **\[**[**control**](control.md)**\]**, and **\[**[**hidden**](hidden.md)**\]**.

</dd> <dt>

*classname* 
</dt> <dd>

Specifies the name by which the component object is known in the type library.

</dd> <dt>

*coclass-definition* 
</dt> <dd>

Specifies statements that make up the [**coclass**](coclass.md) definition.

</dd> </dl>

## Remarks

Licensing is a feature of COM that provides control over object creation. Licensed objects can be created only by clients that are authorized to use them. Licensing is implemented in COM through the [**IClassFactory2**](c49c7612-3b1f-4535-baf3-8458b3f34f95) interface and by support for a license key that can be passed at run time.

### Flags

TYPEFLAG\_FLICENSED

## Examples

``` syntax
[
    uuid(12345678-1234-1234-1234-123456789ABC), 
    licensed, 
    helpstring("A meaningfulcomment"
]
coclass MyClass
{
    // coclass definition statements
};
```

## See also

<dl> <dt>

[**coclass**](coclass.md)
</dt> <dt>

[Contents of a Type Library](https://msdn.microsoft.com/windows/desktop/76b062d4-1a08-47f5-b4d4-064237cb1372)
</dt> <dt>

[**control**](control.md)
</dt> <dt>

[Generating a Type Library With MIDL](generating-a-type-library-with-midl-2.md)
</dt> <dt>

[**helpstring**](helpstring.md)
</dt> <dt>

[**helpcontext**](helpcontext.md)
</dt> <dt>

[**hidden**](hidden.md)
</dt> <dt>

[ODL File Syntax](https://msdn.microsoft.com/windows/desktop/df7aa86f-1453-4409-939e-788d469d611e)
</dt> <dt>

[TYPEFLAGS](https://msdn.microsoft.com/windows/desktop/bf34cc90-f772-4562-9d18-7cf35aeed41e)
</dt> <dt>

[**version**](version.md)
</dt> </dl>

 

 



