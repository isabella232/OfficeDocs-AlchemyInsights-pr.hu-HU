---
title: Csoport hozzáadása SharePoint-webhelyhez
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750522"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Kapcsolódó webhelyek létrehozása vagy csoportosítása SharePoint Online szolgáltatásban – problémák

A csoporthoz kapcsolódó webhely létrehozásakor vagy ismételt létrehozásakor gyakran előforduló problémák merültek fel.

 Ha törölt egy csoportot és a hozzá tartozó webhelyet, és egy másik webhelyet szeretne létrehozni ugyanazzal az URL-címmel, akkor véglegesen el kell távolítania az előző webhelyet.

Letöltés [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 További információ a PowerShell használatbaveléshez: [Ismerkedés a SharePoint Online Management Shell alkalmazással](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Vegye ki a webhelyet a törölt webhelyekről a [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell parancsmaggal.

Ha csoportos kapcsolatban lévő webhelyet hoz létre, és figyelmeztetést kap, akkor már létezik egy másik, azonos aliasnévvel rendelkező csoport, és az Office 365 már meglévő csoportjait is ellenőrzi [a felügyeleti központból](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). A probléma megoldásához törölje a meglévő csoportot, ha már nincs rá szükség, vagy hozza létre a webhelyet egy másik aliasnévvel.

Különböző módokon hozhatók létre és használhatók a SharePoint rendszerben a modern csoportok.

A meglévő webhelyeket összekapcsolhatja egy Office 365-csoporttal. További információ: [Office 365-csoport csatlakoztatása a SharePoint-felhasználó ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Egy Office 365-csoporthoz kapcsolódó webhely létrehozásához létre kell hoznia egy csoportwebhelyet. További információt a [csoportwebhely létrehozása a SharePoint szolgáltatásban](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)című témakörben talál.

