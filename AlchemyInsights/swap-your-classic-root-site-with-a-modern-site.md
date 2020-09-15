---
title: A klasszikus root webhely cseréje modern webhellyel
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691181"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>A klasszikus root webhely cseréje modern webhellyel

Ha a környezete az 2019 áprilisa előtt volt beállítva, a Microsoft PowerShell segítségével módosíthatja a legfelső szintű webhelyet a modern webhelyekhez:

- Ha egy másik webhelyet szeretne használni a legfelső szintű webhelyként, lecserélheti [(felcserélheti) a legfelső szintű webhelyét](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - A [SPOSiteSwap hivatkozhat](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) arra, hogy a webhely helyét egy másik webhelyre cseréli az eredeti webhely archiválása közben. Mindkét csoportwebhely számára elérhető (nem kapcsolódhat egy csoporthoz) és egy kommunikációs webhelyhez. 

- A további lehetőségeket hamarosan bevezetjük, amelyek lehetővé teszik a webhely tartalmának használatát, de a meglévő webhelyet konvertálja egy kommunikációs webhelyre. 
>[!Important]
>Ezek a funkciók fokozatosan jelennek meg. Továbbra is ellenőrizze az üzenetközpont frissítéseit. 

## <a name="known-issues-with-swapping-sites"></a>A webhelyek cseréjével kapcsolatos ismert problémák

- Előfordulhat, hogy a cél egy rövid időre "not found" (HTTP 404) hibát ad vissza.
- A keresési index frissítéséhez a tartalmat újra kell bejárni. Nincs szükség kézi lépésre – ezt automatikusan elvégzi a program.
- A "statikus" hivatkozásokkal (például a fájlok szinkronizálására és a OneNote-fájlokra) függő bármit manuálisan kell kijavítani.
- Ha a forrás webhelye szervezeti hírkiszolgáló volt, frissítse az URL-címet.Az összes szervezeti híroldalak listájának beszerzése.
- Előfordulhat, hogy a Project Server-webhelyek érvényesítése szükséges ahhoz, hogy a rendszer továbbra is megfelelően társítsa őket.
