---
Description: MinWordlistBattery
ms.assetid: 23ea49c3-3607-415c-b086-a4a9ead7ce9e
title: MinWordlistBattery
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# MinWordlistBattery

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

The **MinWordlistBattery** entry is the minimum percentage of battery life remaining to keep indexing active on the computer.

### Summary



|          |                                       |
|----------|---------------------------------------|
| Type:    | **REG\_DWORD**                        |
| Units:   | Percent                               |
| Default: | 100 (never run indexing on batteries) |
| Range:   | 0 - 100                               |



 

### Remarks

To prevent indexing from occurring for battery-powered computers, use the default value of 100 percent. Indexing Service continues to process queries even when not indexing files.

## Related topics

<dl> <dt>

[Catalog, Property, and Scope Registry Entries](catalog--property--and-scope-registry-entries.md)
</dt> <dt>

[Main Registry Entries](main-registry-entries.md)
</dt> </dl>

 

 


