---
title: Nem lehet törölni az elemeket a SharePointban vagy a OneDrive-ban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571261"
---
# <a name="unable-to-delete-items"></a>Nem lehet törölni az elemeket

Az adatmegőrzési házirendek okozhatják ezt, le kell tiltania vagy ki kell zárnia a problémát okozó megfelelő tartást. Az adatmegőrzési szabályzat vagy a letartás eltávolítása után akár 24 órát is igénybe vehet a módosítás érvénybe léptetése. Győződjön meg arról, hogy nincs [adatmegőrzési házirend](https://docs.microsoft.com/office365/securitycompliance/retention-policies) beállítása az elemen.

Lehet, hogy a hely túllépte a tárhelykorlátot, növelte a [helykvótát,](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) és törölheti az elemet.

Győződjön meg arról, hogy az elemet nem [vette ki](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) egy másik felhasználó.

Végül a rendszergazdák [használhatják a SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) függvényt, amely a PowerShell-parancsok tárát tartalmazza, amely lehetővé teszi összetett felügyeleti műveletek, például a makacs elemek kényszerítésének végrehajtásához.
- [PNP-fájl eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-mappa eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-listaelem eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-lista eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-mező eltávolítása (oszlop)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)