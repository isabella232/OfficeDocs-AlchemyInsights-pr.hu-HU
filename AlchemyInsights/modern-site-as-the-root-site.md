---
title: A modern weboldal a gyökérwebhely
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054704"
---
# <a name="modern-site-as-root-site"></a>A modern weboldal mint Gyökéroldal

Megkezdtük a kínálatból egy új funkció, amely lehetővé teszi, hogy a [swap a klasszikus webhely gyökere egy modern oldalon](https://docs.microsoft.com/sharepoint/modern-root-site). Az [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) használata segítségével kicserélheti egy webhely helyét egy másik webhelyre az eredeti webhely archiválása közben. Elérhető mindkét csoportwebhelyhez (nem kapcsolódik csoporthoz) és kommunikációs webhelyhez.

>[!Important]
> A klasszikus gyökérwebhelyet ne törölje, hogy modern kommunikációs webhelyet hozzon létre. Ezt a Microsoft nem támogatja. A gyökérwebhely törlésével minden felhasználó számára hozzáférhetetlenné válik a szervezet összes SharePoint-webhelye, amíg vissza nem állítja a webhelyet, vagy ha ugyanazon az URL-címen új webhelyet hoz létre. Mi lesz kommunikálni ezt a funkciót keresztül az üzenetközpont. A szolgáltatás hamarosan bekapcsolódik a bérlőbe.

## <a name="known-issues-with-swapping-sites"></a>A helyek swapping ismert problémái
- A célwebhely rövid ideig "nem található" (HTTP 404) hibát ad vissza.
- A keresési index frissítéséhez a tartalmat recrawled kell. Nincs kézi lépés szükséges itt, ez automatikusan megtörténik.
- A "statikus" hivatkozásokra (például a fájlszinkronizálás és a OneNote-fájlok) vonatkozó bármit manuálisan kell javítani.
- Előfordulhat, hogy a Project Server webhelyeit érvényesíteni kell annak érdekében, hogy még mindig helyesen legyenek társítva. 
