---
title: Csoport hozzáadása SharePoint-webhelyhez
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
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44064395"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problémák a csoportos csatlakoztatott webhely SharePoint-ban történő létrehozásakor

1. A csoporthoz csatlakoztatott hely létrehozása vagy újbóli létrehozása során gyakran előforduló gyakori problémák.
Ha törölt egy csoportot és annak csatlakoztatott webhelyét, és egy másik webhelyet szeretne létrehozni ugyanazzal az URL-címmel, véglegesen el kell távolítania az előző webhelyet.

   - [SPO-felügyeleti rendszerhéj](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) letöltése
   - A PowerShell kezelésének megkezdéséről a [SharePoint Online Felügyeleti rendszerhéj – első lépések](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)ebben az esetben olvashat bővebben.
   - Távolítsa el a helyet a törölt helyekről az [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell parancsmag használatával. A Powershell szükséges a csoportwebhelyek végleges törléséhez.

1. Ha csoporthoz csatlakoztatott webhelyet hoz létre, és figyelmeztetést kap: **Már létezik egy másik, azonos aliassal rendelkező csoport,** ellenőrizze a meglévő csoportokat a [Microsoft 365 Felügyeleti központból.](https://admin.microsoft.com/AdminPortal/Home#/groups) A probléma megoldásához törölje a meglévő csoportot, ha már nincs rá szükség, vagy hozzon létre egy másik aliast hozzárendelt webhelyet.

1. A SharePoint segítségével különböző módokon hozhat létre és használhat modern csoportokat.

   - Meglévő helyeket microsoft 365-csoporthoz kapcsolhat. További információt a [Microsoft 365-csoport csatlakoztatása a SharePoint felhasználói felületén című témakörben](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)talál.
   - Microsoft 365 csoporthoz csatlakoztatott webhely létrehozásához [csoportwebhelyet kell létrehoznia.](https://admin.microsoft.com/sharepoint)
