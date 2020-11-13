---
title: Nem lehet elemeket törölni a SharePointban vagy a OneDrive-ban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019585"
---
# <a name="unable-to-delete-items"></a>Nem lehet elemeket törölni

- Az adatmegőrzési házirendek ezt a problémát okozhatják, le kell tiltania vagy ki kell zárnia a problémát okozó megfelelő mentességet. Az adatmegőrzési házirend vagy a mentesség eltávolítása után akár 24 óra is eltelhet, amíg a módosítás érvénybe lép. Ügyeljen arra, hogy az elemen ne legyen [adatmegőrzési házirend](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) -beállítás.

- Előfordulhat, hogy a webhely túllépte a tárterület korlátozását, megnöveli a [webhely kvótáját](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) , és törli az elemet.

- Ügyeljen arra, hogy az elem ne legyen [kivéve](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) egy másik felhasználónál.

- Végül a rendszergazdák használhatják a [SharePoint-mintákat és-eljárásokat](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), amelyek egy PowerShell-parancsok gyűjteményét tartalmazzák, amelyek lehetővé teszik az összetett kezelési műveletek végrehajtását, például a makacs elemek törlésének kényszerítését.
- [A PNP-fájl eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-mappa eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [A PNP-listaelem eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [A PNP-lista eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [A PNP-mező (oszlop) eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)