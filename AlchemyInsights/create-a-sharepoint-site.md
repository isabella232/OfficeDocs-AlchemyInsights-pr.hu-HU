---
title: SharePoint-webhely létrehozása
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
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806941"
---
# <a name="create-a-sharepoint-site"></a>SharePoint-webhely létrehozása

Webhelyek létrehozása és kezelése az [aktív webhelyekről](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) a SharePoint felügyeleti központban. További információt [a webhelyek kezelése az új SharePoint felügyeleti központban](https://docs.microsoft.com/sharepoint/manage-site-creation)című témakörben talál. 

## <a name="tips"></a>Tippek

- A meglévő webhelyek URL-címét tartalmazó webhelyek **nem** hozhatók létre. Ha törölt egy webhelyet, és az URL-címet újra szeretné használni, lehetséges, hogy a törölt webhely továbbra is megtalálható a [törölt webhelyek](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)csoportban. A webhelyet véglegesen törölni kell az URL-cím ismételt felhasználásához. Ha teljesen el szeretné távolítani a PowerShell-webhelyet, tekintse át a [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) parancsmagot.
- Előfordulhat, hogy bizonyos felhasználók nem tudnak webhelyeket létrehozni. [Lásd: webhelykészítés kezelése a SharePoint Online-ban](https://docs.microsoft.com/sharepoint/manage-site-creation).
- Lehetséges, hogy a webhely megakad a **vártnál hosszabb ideig** . Ha több mint 24 óra telt el, mióta először látta ezt a problémát, kérjük, jelentkezzen be egy támogatási jegybe. Sok esetben már dolgozunk a megoldáson. Kérjük, hogy végezze el a megfelelő megoldást legalább 24 óráig.
