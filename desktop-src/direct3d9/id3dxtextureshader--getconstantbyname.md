---
Description: Gets a constant by looking up its name.
ms.assetid: 0c57f6ce-ea81-4b34-9251-c385bfe6ebe7
title: ID3DXTextureShader::GetConstantByName method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- ID3DXTextureShader.GetConstantByName
api_type: 
- COM
api_location: 
- d3dx9.lib
- d3dx9.dll
---

# ID3DXTextureShader::GetConstantByName method

Gets a constant by looking up its name.

## Syntax


```C++
D3DXHANDLE GetConstantByName(
  [in] D3DXHANDLE hConstant,
  [in] LPCSTR     pName
);
```



## Parameters

<dl> <dt>

*hConstant* \[in\]
</dt> <dd>

Type: **[D3DXHANDLE](dx9-graphics-reference-effects-constants.md)**

A [handle](handles.md) to the parent data structure. If the constant is a top-level parameter (there is no parent data structure), use **NULL**.

</dd> <dt>

*pName* \[in\]
</dt> <dd>

Type: **[**LPCSTR**](https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx)**

A string containing the name of the constant.

</dd> </dl>

## Return value

Type: **[D3DXHANDLE](dx9-graphics-reference-effects-constants.md)**

Returns a unique identifier to the constant.

## Requirements



|                    |                                                                                          |
|--------------------|------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Shader.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>     |



## See also

<dl> <dt>

[ID3DXTextureShader](id3dxtextureshader.md)
</dt> </dl>

 

 



