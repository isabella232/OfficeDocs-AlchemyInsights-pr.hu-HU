---
title: Csoport felvétele SharePoint-webhelyre
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771206"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problémák a csoporthoz csatlakoztatott SharePoint-webhelyek létrehozásakor

1. A csoporttal összekapcsolt webhelyek létrehozásakor vagy ismételt létrehozásakor előforduló gyakori problémák.
Ha törölt egy csoportot és a hozzá kapcsolódó webhelyet, és egy URL-lel másik webhelyet szeretne létrehozni, akkor véglegesen el kell távolítania az előző webhelyet.

   - A [Spongya felügyeleti rendszerhéj](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) letöltése
   - A PowerShell használatáról további információt a [SharePoint Online felügyeleti rendszerhéj – első lépések](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)című témakörben találhat.
   - Távolítsa el a webhelyet a törölt webhelyekről a [Remove-SPODeletedSite PowerShell-](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) parancsmag használatával. A csoport webhelyeinek végleges törléséhez PowerShell szükséges.

1. Ha egy csoporthoz kapcsolt webhelyet hoz létre, és figyelmeztetést jelenít meg: **egy másik, ugyanazzal az aliassal rendelkező csoport már létezik**, ellenőrizze a [Microsoft 365 felügyeleti központjának](https://admin.microsoft.com/AdminPortal/Home#/groups)meglévő csoportját. A probléma megoldásához törölje a meglévő csoportot, ha már nincs rá szükség, vagy hozza létre azt a webhelyet, amelyhez másik alias van rendelve.

1. A modern csoportokat többféle módon hozhatja létre és használhatja a SharePointtal.

   - A meglévő webhelyeket összekapcsolhatja a Microsoft 365-csoporttal. További információt a [Microsoft 365-csoport csatlakoztatása a SharePoint felhasználói felületéről](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)című témakörben találhat.
   - Ha létre szeretne hozni egy Microsoft 365-csoportot tartalmazó összekapcsolt webhelyet, létre kell hoznia egy [csoportwebhely](https://admin.microsoft.com/sharepoint)-webhelyet.
