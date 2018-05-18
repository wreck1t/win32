﻿---
Description: 'Computes a coordinate-axis oriented bounding box.'
ms.assetid: '74e1b84e-1264-49eb-9172-7842af7e25e0'
title: D3DXComputeBoundingBox function
---

# D3DXComputeBoundingBox function

Computes a coordinate-axis oriented bounding box.

## Syntax


```C++
HRESULT D3DXComputeBoundingBox(
  _In_  const D3DXVECTOR3 *pFirstPosition,
  _In_        DWORD       NumVertices,
  _In_        DWORD       dwStride,
  _Out_       D3DXVECTOR3 *pMin,
  _Out_       D3DXVECTOR3 *pMax
);
```



## Parameters

<dl> <dt>

*pFirstPosition* \[in\]
</dt> <dd>

Type: **const [**D3DXVECTOR3**](d3dxvector3.md)\***

Pointer to the first position.

</dd> <dt>

*NumVertices* \[in\]
</dt> <dd>

Type: **[**DWORD**](winprog.windows_data_types)**

Number of vertices.

</dd> <dt>

*dwStride* \[in\]
</dt> <dd>

Type: **[**DWORD**](winprog.windows_data_types)**

Count or number of bytes between vertices.

</dd> <dt>

*pMin* \[out\]
</dt> <dd>

Type: **[**D3DXVECTOR3**](d3dxvector3.md)\***

Pointer to a [**D3DXVECTOR3**](d3dxvector3.md) structure, describing the returned lower-left corner of the bounding box. See Remarks.

</dd> <dt>

*pMax* \[out\]
</dt> <dd>

Type: **[**D3DXVECTOR3**](d3dxvector3.md)\***

Pointer to a [**D3DXVECTOR3**](d3dxvector3.md) structure, describing the returned upper-right corner of the bounding box. See Remarks.

</dd> </dl>

## Return value

Type: **[**HRESULT**](455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

If the function succeeds, the return value is D3D\_OK. If the function fails, the return value can be one of the following: D3DERR\_INVALIDCALL.

## Remarks

## Requirements



|                    |                                                                                        |
|--------------------|----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Mesh.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>   |



## See also

<dl> <dt>

[Mesh Functions](dx9-graphics-reference-d3dx-functions-mesh.md)
</dt> </dl>

 

 



