---
title: A Microsoft Edge használata a eDiscovery exportálásához a Chromium böngészők alapján
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 64aebb7f048dba37eef8cd1fa6286b36823d3f0f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734517"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>A Microsoft Edge használata a eDiscovery exportálásához a Chromium böngészők alapján

A legutóbbi változtatások miatt a Microsoft Edge böngészőknek alapértelmezés szerint nincs engedélyezve a ClickOnce támogatása. A Microsoft 365 eDiscovery exportálási eszközének folytatásához a Microsoft Internet Explorer böngészőt kell használnia, vagy engedélyeznie kell a ClickOnce támogatást a Microsoft Edge-ben. 

A ClickOnce támogatás engedélyezése a Microsoft Edge-ben a Chromium alapján: 
1. A Microsoft Edge böngészőjében keresse fel a edge://flags/#edge – egyszer.
2. A ClickOnce támogatás beállításnál módosítsa az **alapértelmezett** vagy a **letiltott** érték beállítás értékét az **engedélyezve**értékre. 
3. A böngészőablak alján válassza az **Újraindítás**gombot. <br>
 A módosítások a Microsoft Edge újraindítása után lépnek életbe. 

Az exportálási eszköz telepítésével kapcsolatos további tudnivalókért olvassa el a tartalmi találatok [ exportálása](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)című témakört.