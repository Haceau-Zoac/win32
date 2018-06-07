---
Description: Retrieves albedo values of the mesh vertices.
ms.assetid: 12b8d6d1-c806-4dcd-80ac-f3963215dcf4
title: ID3DXPRTEngine::GetVertexAlbedo method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# ID3DXPRTEngine::GetVertexAlbedo method

Retrieves albedo values of the mesh vertices.

## Syntax


```C++
HRESULT GetVertexAlbedo(
  [in, out] D3DXCOLOR *pVertColors,
  [in]      UINT      NumVerts
);
```



## Parameters

<dl> <dt>

*pVertColors* \[in, out\]
</dt> <dd>

Type: **[**D3DXCOLOR**](d3dxcolor.md)\***

Pointer to a destination array of albedo values of the mesh vertices. See [**D3DXCOLOR**](d3dxcolor.md).

</dd> <dt>

*NumVerts* \[in\]
</dt> <dd>

Type: **[**UINT**](https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46)**

Number of vertices in the mesh.

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/windows/desktop/455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

If the method succeeds, the return value is S\_OK. If the method fails, the return value can be one of the following: D3DERR\_INVALIDCALL, E\_OUTOFMEMORY.

## Requirements



|                    |                                                                                        |
|--------------------|----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Mesh.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>   |



## See also

<dl> <dt>

[ID3DXPRTEngine](id3dxprtengine.md)
</dt> </dl>

 

 



