---
title: A klasszikus Modern webhely legfelső szintű webhely felcserélése
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501081"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>A klasszikus Modern webhely legfelső szintű webhely felcserélése

A környezet április 2019 előtt hozták létre, ha a Microsoft PowerShell használatával módosíthatja a legfelső szintű webhely modern webhely:

- Ha a legfelső szintű webhely használni kívánt másik helyre, (swap) a legfelső szintű webhely cserélheti vele. 
    - [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) segítségével felcserélése egy másik webhelyet a webhely helyét az eredeti helyre archiválás során. A csoportwebhely (nem kapcsolódik egy csoport) és a kommunikációs hely áll rendelkezésre. 

- További lehetőségeket fogják bevezetni legrövidebb időn belül, amely lehetővé teszi a tovább használni a tartalmat a webhelyen, de a meglévő webhely átalakítása kommunikációs hely. 
>[!Important]
>Ezek a funkciók lesznek-e vetítve fokozatosan. Továbbra is az Office 365 Message Center frissítések ellenőrzése. 

## <a name="known-issues-with-swapping-sites"></a>Csere helyek kapcsolatos ismert problémák

- A célwebhely vissza "nem található" hiba (HTTP 404) egy rövid ideig.
- Tartalom kell frissíteni a keresési indexben kell recrawled. Nincs szükség kézi lépés van – ez automatikusan történik.
- Semmit sem függ a "statikus" hivatkozások (például fájlszinkronizálás és a OneNote-fájlok) manuálisan kell javítani kell.
- Ha a forráswebhely egy szervezeti híreket tartalmazó webhely volt, az URL-cím frissítéseSzervezeti hírcsoporthelyek listájának megjelenítése.
- A Project Server-webhelyek kell annak biztosítása érdekében, hogy még az társított érvényesíthető.





