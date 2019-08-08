---
title: A modern webhelyre, ahol a legfelső szintű webhely
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232717"
---
# <a name="modern-site-as-root-site"></a>A modern webhelyre, ahol a legfelső szintű webhely

Ezért megkezdődött, bevezetés egy új szolgáltatás, amely lehetővé teszi, hogy a klasszikus webhely legfelső szintű webhely modern hellyel felcserélése. [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) segítségével felcserélése egy másik webhelyet a webhely helyét az eredeti helyre archiválás során. A csoportwebhely (nem kapcsolódik egy csoport) és a kommunikációs hely áll rendelkezésre. 

>[!Important]
> Ne törölje a klasszikus legfelső szintű webhely a modern kommunikációs webhelyet hozhat létre. Ez a Microsoft által nem támogatott. A legfelső szintű webhely törlése tesz minden SharePoint-webhely a szervezet nem érhető el minden felhasználó számára addig, amíg a webhely visszaállítása, vagy hozzon létre egy új helyet azonos URL-címen. Fogja azt közlő üzenet közepén keresztül ezt a szolgáltatást. A funkció segítségével kapcsolható be a bérlő röviddel számíthatunk.

## <a name="known-issues-with-swapping-sites"></a>Csere helyek kapcsolatos ismert problémák
- A célwebhely vissza "nem található" hiba (HTTP 404) egy rövid ideig.
- Tartalom kell frissíteni a keresési indexben kell recrawled. Nem szükséges itt kézi művelet van, ez automatikusan megtörténik.
- Semmit sem függ a "statikus" hivatkozások (például fájlszinkronizálás és a OneNote-fájlok) manuálisan kell javítani kell.
- A Project Server-webhelyek kell annak biztosítása érdekében, hogy még az társított érvényesíthető. 
