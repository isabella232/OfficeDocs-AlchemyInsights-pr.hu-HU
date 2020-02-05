---
title: Csoport felvétele SharePoint-webhelyre
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770353"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problémák a csoporthoz kapcsolódó webhely SharePointban történő létrehozásakor

1. Néhány gyakori probléma, amely a csoporthoz kapcsolódó webhely létrehozásakor vagy újbóli létrehozásakor merült fel.
Ha törölt egy csoportot és a kapcsolódó webhelyet, és egy másik webhelyet szeretne létrehozni ugyanazzal az URL-címmel, véglegesen el kell távolítania az előző webhelyet.

   - [SPO felügyeleti rendszerhéj](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) letöltése
   - A Powershell használatával kapcsolatos további tudnivalókért olvassa el [a SharePoint Online Felügyeleti rendszerhéj első](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)lépései .
   - Távolítsa el a webhelyet a törölt helyekről az [Eltávolítás-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell-parancsmag használatával. A Powershell szükséges a csoporthelyek végleges törléséhez.

1. Ha csoporthoz kapcsolódó webhelyet hoz létre, és figyelmeztetést kap: **Már létezik egy másik, ugyanazzal az aliasnevű csoport,** ellenőrizze a meglévő csoportokat az [Office 365-ből a Felügyeleti központból.](https://admin.microsoft.com/AdminPortal/Home#/groups) A probléma megoldásához törölje a meglévő csoportot, ha már nincs rá szükség, vagy hozzon létre egy másik aliast.

1. A SharePoint tal különböző módokon hozhat létre és használhat modern csoportokat.

   - A meglévő webhelyeket office 365-csoporthoz csatlakoztathatja. További információt [az Office 365-csoport csatlakoztatása a SharePoint felhasználói felületével](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)című témakörben talál.
   - Office 365-csoporthoz kapcsolódó webhely létrehozásához létre kell hoznia egy [csoportwebhelyet.](https://admin.microsoft.com/sharepoint)
