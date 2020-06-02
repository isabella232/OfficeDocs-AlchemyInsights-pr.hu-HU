---
title: Nem lehet törölni az elemeket a SharePointban vagy a OneDrive-on
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511978"
---
# <a name="unable-to-delete-items"></a>Nem lehet törölni az elemeket

Az adatmegőrzési házirendek ezt okozhatják, le kell tiltania vagy ki kell zárnia a problémát okozó megfelelő visszatartást. Az adatmegőrzési szabály vagy a visszatartás eltávolítása után akár 24 órát is igénybe vehet, amíg a módosítás érvénybe lép. Győződjön meg arról, hogy nincs [adatmegőrzési házirend](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) beállítása a cikken.

Előfordulhat, hogy a hely túllépte a tárolási korlátot, növelheti a [helykvótát,](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) és törölheti az elemet.

Győződjön meg arról, hogy az elemet nem [vette ki](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) egy másik felhasználónak.

Végül a rendszergazdák [használhatják a SharePoint Minták és gyakorlatok](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), amely egy könyvtár a PowerShell-parancsok, amelyek lehetővé teszik, hogy összetett felügyeleti műveletek, például a makacs elemek kényszerítése.
- [PNP-fájl eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-mappa eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-listaelem eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-lista eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-mező eltávolítása (oszlop)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)