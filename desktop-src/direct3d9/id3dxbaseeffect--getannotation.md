﻿---
Description: 'Gets the handle of an annotation.'
ms.assetid: '433d73b7-9371-4d76-8b34-a64c608eb1a3'
title: 'ID3DXBaseEffect::GetAnnotation method'
---

# ID3DXBaseEffect::GetAnnotation method

Gets the handle of an annotation.

## Syntax


```C++
D3DXHANDLE GetAnnotation(
  [in] D3DXHANDLE hObject,
  [in] UINT       Index
);
```



## Parameters

<dl> <dt>

*hObject* \[in\]
</dt> <dd>

Type: **[D3DXHANDLE](dx9-graphics-reference-effects-constants.md)**

Handle of a technique, pass, or top-level parameter. See [Handles (Direct3D 9)](handles.md).

</dd> <dt>

*Index* \[in\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

Annotation index.

</dd> </dl>

## Return value

Type: **[D3DXHANDLE](dx9-graphics-reference-effects-constants.md)**

Returns the handle of the specified annotation, or **NULL** if the index was invalid. See [Handles (Direct3D 9)](handles.md).

## Remarks

Annotations are user-specific data that can be attached to any technique, pass, or parameter. See [Handles (Direct3D 9)](handles.md).

## Requirements



|                    |                                                                                          |
|--------------------|------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Effect.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>     |



## See also

<dl> <dt>

[ID3DXBaseEffect](id3dxbaseeffect.md)
</dt> </dl>

 

 



