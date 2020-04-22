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
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642146"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problémák a csoportos csatlakoztatott webhely SharePoint-ban történő létrehozásakor

1. A csoporthoz csatlakoztatott hely létrehozása vagy újbóli létrehozása során gyakran előforduló gyakori problémák.
Ha törölt egy csoportot és annak csatlakoztatott webhelyét, és egy másik webhelyet szeretne létrehozni ugyanazzal az URL-címmel, véglegesen el kell távolítania az előző webhelyet.

   - [SPO-felügyeleti rendszerhéj](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) letöltése
   - A PowerShell kezelésének megkezdéséről a [SharePoint Online Felügyeleti rendszerhéj – első lépések](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)ebben az esetben olvashat bővebben.
   - Távolítsa el a helyet a törölt helyekről az [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell parancsmag használatával. A Powershell szükséges a csoportwebhelyek végleges törléséhez.

1. Ha csoporthoz csatlakoztatott webhelyet hoz létre, és figyelmeztetést kap: **Már létezik egy másik, azonos aliassal rendelkező csoport,** ellenőrizze a meglévő csoportokat a [Microsoft 365 Felügyeleti központban.](https://admin.microsoft.com/AdminPortal/Home#/groups) A probléma megoldásához törölje a meglévő csoportot, ha már nincs rá szükség, vagy hozzon létre egy másik aliast hozzárendelt webhelyet.

1. A SharePoint segítségével különböző módokon hozhat létre és használhat modern csoportokat.

   - Meglévő webhelyeket kapcsolhat egy Office 365-csoporthoz. További információt az [Office 365-ös csoport csatlakoztatása a SharePoint felhasználói felületén című témakörben](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)talál.
   - Office 365-ös csoporthoz csatlakoztatott webhely létrehozásához [csoportwebhelyet kell létrehoznia.](https://admin.microsoft.com/sharepoint)
