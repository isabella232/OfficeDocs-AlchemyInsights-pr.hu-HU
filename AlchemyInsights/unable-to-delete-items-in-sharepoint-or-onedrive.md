---
title: Nem lehet elemeket törölni a SharePoint és a OneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038519"
---
# <a name="unable-to-delete-items"></a>Nem lehet elemeket törölni

- Ezt az adatmegőrzési házirendek okozhatják, ezért vagy le kell tiltania vagy ki kell zárnia a vonatkozó visszatartást, amely a problémát okozza. Az adatmegőrzési házirend vagy visszatartás eltávolítása után akár 24 óra is elehet, hogy a módosítás életbe lép. Győződjön meg arról, hogy [az](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) elemhez nincs adatmegőrzési házirend beállítva.

- Előfordulhat, hogy a webhely túllépte a tárterületkorlátot, megnövelte a [webhelykvótát,](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) és törölte az elemet.

- Győződjön meg arról, hogy az elem [nincs kivett másik](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) felhasználónak.

- Végül [SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) a rendszergazdák a PnP (PnP) használatával is végezhetnek műveleteket, amelyek powershell-parancsokat tartalmaznak, így összetett felügyeleti műveleteket hajthat végre, például felesleges elemeket törölhet.
- [PNP-fájl eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-mappa eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-listaelem eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-lista eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP mező (oszlop) eltávolítása](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)