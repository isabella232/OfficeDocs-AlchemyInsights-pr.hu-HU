---
title: A klasszikus gyökérwebhely felcserélése egy modern webhelyre
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741546"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>A klasszikus gyökérwebhely felcserélése egy modern webhelyre

Ha a környezet 2019 áprilisa előtt lett beállítva, a Microsoft PowerShell használatával modern webhelyre módosíthatja a gyökérwebhelyet:

- Ha van egy másik webhely, amelyet gyökérwebhelyként szeretne használni, lecserélheti [(cserélheti) a gyökérwebhelyet.](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - [Az Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) segítségével az eredeti webhely archiválása közben cserélheti fel a webhely helyét egy másik hellyel. A csoportwebhelyhez (csoporthoz nem kapcsolódó) és a kommunikációs helyhez egyaránt elérhető. 

- Hamarosan további képességek kerülnek bevezetésre, amelyek lehetővé teszik a webhely tartalmának további használatát, de a meglévő webhelyet kommunikációs webhelyre konvertálhatja. 
>[!Important]
>Ezek a képességek fokozatosan kerülnek bevezetésre. Folytassa a frissítéseket az Üzenetközpontban. 

## <a name="known-issues-with-swapping-sites"></a>Ismert problémák a webhelyek cseréjével kapcsolatban

- A célwebhely rövid ideig "nem található" (HTTP 404) hibát adhat vissza.
- A keresési index frissítéséhez a tartalmat újra kell feltérképezni. Nincs szükség manuális lépésre - ez automatikusan történik.
- A "statikus" hivatkozásoktól (például a Fájlszinkronizálástól és a OneNote-fájloktól) függő minden hivatkozást manuálisan kell kijavítani.
- Ha a forráswebhely szervezeti hírwebhely volt, frissítse az URL-címet.Az összes szervezeti híroldal listájának beszereznie.
- Előfordulhat, hogy a Project kiszolgáló helyhelyeit ellenőrizni kell annak érdekében, hogy azok továbbra is megfelelően legyenek társítva.
