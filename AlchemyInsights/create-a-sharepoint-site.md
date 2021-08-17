---
title: Webhely SharePoint létrehozása
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080892"
---
# <a name="create-a-sharepoint-site"></a>Webhely SharePoint létrehozása

Webhelyeket hozhat létre vagy kezelhet az aktív [webhelyek közül](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) SharePoint Felügyeleti központban. További információt a Webhelyek kezelése az új felügyeleti [SharePoint című témakörben.](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>Tippek:

- Meglévő **webhely** URL-címével nem hozhat létre webhelyet. Ha törölt egy webhelyet, és újra fel szeretné használni az URL-címet, lehetséges, hogy a törölt webhely továbbra is létezik a Törölt [webhelyek csoportban.](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) Az URL-cím újrahasználata előtt a webhelyet véglegesen törölni kell. Ha teljesen el szeretne távolítani egy webhelyet a Powershell használatával, tekintse meg a [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) parancsmag példáját.
- Előfordulhat, hogy egyes felhasználók nem tudnak webhelyet létrehozni. [Lásd: Webhelykészítés kezelése a SharePoint Online-ban.](https://docs.microsoft.com/sharepoint/manage-site-creation)
- Lehetséges, hogy a webhely a  vártnál tovább tart a létrehozásnál. Ha a probléma első jelentkezte óta több mint 24 óra telt el, kérjük, írjon be egy támogatási jegyet. Sok esetben már dolgozunk a megoldáson. Kérjük, várjon legalább 24 órát a megoldásunkra.
