---
title: Csoport hozzáadása SharePoint webhelyhez
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318126"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Gyakori problémák a csoporthoz csatlakoztatott webhely létrehozásakor a SharePoint

1. Ha törölt egy csoportot és annak csatlakoztatott webhelyét, és szeretne egy másik webhelyet létrehozni ugyanazokkal az URL-címekkel, véglegesen el kell távolítania az előző webhelyet.

   - [SPO felügyeleti rendszerhéj letöltése](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - A Powershell használatával kapcsolatos első lépésekről további információt Az SharePoint Management Shell – első lépések [SharePoint.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Távolítsa el a webhelyet a Törölt webhelyek webhelyről a [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell-parancsmag használatával. A csoport webhelyek végleges törléséhez Powershellre van szükség.

1. Ha csoporthoz csatlakoztatott webhelyet hoz létre, és a következő figyelmeztetés jelenik **meg:** Már létezik egy másik csoport azonos aliassal, ellenőrizze a meglévő csoportokat a [Microsoft 365 Felügyeleti központ.](https://admin.microsoft.com/AdminPortal/Home#/groups) A probléma megoldásához törölje a már meglévő csoportot, ha már nincs rá szükség, vagy hozzon létre egy másik aliassal társított webhelyet.

1. A modern csoportok különböző módokon hozhatók létre és használhatók SharePoint.

   - A meglévő webhelyeket összekapcsolhatja egy Microsoft 365 csoporttal. További információért lásd: Csatlakozás csoport Microsoft 365 a felhasználói SharePoint [használatával.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Ha csapatcsoporthoz Microsoft 365 webhelyet, létre kell hoznia egy [csapatwebhelyet.](https://admin.microsoft.com/sharepoint)
