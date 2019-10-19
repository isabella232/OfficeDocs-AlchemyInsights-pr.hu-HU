---
title: Nem lehet törölni az elemeket a SharePoint vagy az OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748561"
---
# <a name="unable-to-delete-items"></a>Az elemek nem törölhetők

Problémák vannak a SharePoint-elemek törlésével?

- Mindig győződjön meg arról, hogy rendelkezik a [megfelelő engedélyekkel](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) az elem törléséhez, vagy ha a [webhelycsoport rendszergazdája](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) megkísérli eltávolítani az elemet.

- Ellenőrizze, hogy nincs-e az [adatmegőrzési házirend](https://docs.microsoft.com/office365/securitycompliance/retention-policies) beállítása a elemen.

- Győződjön meg arról, hogy az elemet nem egy másik felhasználó [vette ki](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) .

- Végül, ügyintéző tud használ [SharePoint példa és üzelmek](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) melyik tartalmaz egy könyvtár-ból PowerShell követel amit enged ön-hoz előad összetett vezetés tettek mint kényszerít törlés makacs cikk.
- [PNP-fájl eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-mappa eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-listaelem eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-lista eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP mező eltávolítása (oszlop)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)