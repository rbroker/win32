---
Description: Close the Parent Recordset Object
ms.assetid: a88d77ca-1337-499f-92a9-bf597ea96b01
title: Close the Parent Recordset Object
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Close the Parent Recordset Object

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

This code segment uses the [**Close**](https://www.bing.com/search?q=**Close**) method of the objRS\_Parent [**Recordset**](https://www.bing.com/search?q=**Recordset**) object to free the system resources of the parent recordset. Setting the objRS\_Parent **Recordset** object to Nothing removes the parent object from memory.


```VB
objRS_Parent.Close
objRS_Parent = Nothing
```



 

 


