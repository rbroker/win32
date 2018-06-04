---
Description: Retrieves the data in an index buffer.
ms.assetid: 7e25ad67-7f9d-4c23-a029-a2262034ef38
title: ID3DX10Mesh::GetIndexBuffer method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# ID3DX10Mesh::GetIndexBuffer method

Retrieves the data in an index buffer.

## Syntax


```C++
HRESULT GetIndexBuffer(
  [out] ID3DX10MeshBuffer **ppIndexBuffer
);
```



## Parameters

<dl> <dt>

*ppIndexBuffer* \[out\]
</dt> <dd>

Type: **[**ID3DX10MeshBuffer**](id3dx10meshbuffer.md)\*\***

Address of a pointer to a ID3DX10MeshBuffer interface, representing the index buffer associated with the mesh.

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/windows/desktop/455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

The return value is one of the values listed in [Direct3D 10 Return Codes](d3d10-graphics-reference-returnvalues.md).

## Requirements



|                    |                                                                                       |
|--------------------|---------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX10.h</dt> </dl>   |
| Library<br/> | <dl> <dt>D3DX10.lib</dt> </dl> |



## See also

<dl> <dt>

[ID3DX10Mesh](id3dx10mesh.md)
</dt> <dt>

[D3DX Interfaces](d3d10-graphics-reference-d3dx10-interfaces.md)
</dt> </dl>

 

 



