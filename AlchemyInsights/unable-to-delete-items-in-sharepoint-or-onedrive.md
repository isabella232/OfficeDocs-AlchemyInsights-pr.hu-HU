---
title: Nem lehet törölni a SharePoint- vagy OneDrive cikkek
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057724"
---
# <a name="unable-to-delete-items"></a>Nem törölhető elemek

Elemek törlése a probléma?

- Mindig ellenőrizze, hogy rendelkezik a [megfelelő engedélyekkel](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) , illetve törli az elemet a [webhelycsoport rendszergazdája](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) kísérlet eltávolítja az elemet.

- Győződjön meg arról, hogy nincs olyan [adatmegőrzési szabály](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) beállítása az elemen.

- Ellenőrizze, hogy az elem nem egy másik felhasználó [kivette](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) .

- Végül a rendszergazdák használhatják [SharePoint szokások és gyakorlatok](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) tartalmazó könyvtár PowerShell parancsok, amelyek lehetővé teszik az összetett kezelési műveletek végrehajtásához kényszerítése stubborn elemek törlése. 
- [PNP fájl eltávolítása](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-mappa eltávolítása](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Távolítsa el a PNP listaelem](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP lista törlése](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Távolítsa el a PNP mező (oszlop)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)