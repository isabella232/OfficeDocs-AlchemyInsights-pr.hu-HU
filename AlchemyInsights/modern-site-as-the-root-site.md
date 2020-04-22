---
title: Modern oldal, mint a gyökér hely
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713793"
---
# <a name="modern-site-as-root-site"></a>Modern webhely gyökérhelyként

Elkezdtünk egy új funkciót kivonni, amely lehetővé teszi, hogy [a klasszikus webhely gyökérwebhelyét egy modern webhelyre cserélje.](https://docs.microsoft.com/sharepoint/modern-root-site) [Az Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) segítségével az eredeti webhely archiválása közben cserélheti fel a webhely helyét egy másik hellyel. A csoportwebhelyhez (csoporthoz nem kapcsolódó) és a kommunikációs helyhez egyaránt elérhető.

>[!Important]
> Ne törölje a klasszikus gyökérwebhelyet, hogy modern kommunikációs webhelyet hozzon létre. Ezt a Microsoft nem támogatja. A gyökérwebhely törlésével a szervezet összes SharePoint-webhelye elérhetetlenné válik minden felhasználó számára, amíg vissza nem állítja a webhelyet, vagy nem hoz létre új webhelyet ugyanazon az URL-címen. Ezt a funkciót az üzenetközponton keresztül fogjuk közlöm. Azt kell várni, hogy a szolgáltatás be van kapcsolva a bérlő hamarosan.

## <a name="known-issues-with-swapping-sites"></a>Ismert problémák a webhelyek cseréjével kapcsolatban
- A célwebhely rövid ideig "nem található" (HTTP 404) hibát adhat vissza.
- A keresési index frissítéséhez a tartalmat újra kell feltérképezni. Itt nincs szükség manuális lépésre, ez automatikusan megtörténik.
- A "statikus" hivatkozásoktól (például a Fájlszinkronizálástól és a OneNote-fájloktól) függő minden hivatkozást manuálisan kell kijavítani.
- Előfordulhat, hogy a Project kiszolgáló helyhelyeit ellenőrizni kell annak érdekében, hogy azok továbbra is megfelelően legyenek társítva. 
