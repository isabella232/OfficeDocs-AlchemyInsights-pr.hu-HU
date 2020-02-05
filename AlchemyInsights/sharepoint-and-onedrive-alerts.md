---
title: A SharePoint- és OneDrive-riasztások fogadásának késedelme
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771217"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>A SharePoint- és OneDrive-riasztások fogadásának késedelme

- Először ellenőrizze a Levélszemét vagy levélszemét mappát az e-mailben.
- Ha **több fájlból vagy tárakból származó összes riasztás késik,** látogasson el a [Service Health irányítópultjára,](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) és ellenőrizze, hogy vannak-e olyan tanácsadók/incidensek, amelyek a SharePointban vagy az Exchange-ben fordulhatnak elő. A probléma lehet a SharePoint riasztási képességgel vagy az Exchange-en keresztül küldött e-mailek késésével. Vegye figyelembe azt is, hogy más e-mailek kézbesítése folyamatban van-e – ha nem, akkor a probléma valószínűleg az Exchange késése.
- Ha **egy adott fájlból vagy tárból nem kézbesítegy egyedi riasztást,** próbálja meg törölni és újra létrehozni. A riasztás újbóli létrehozásához olvassa el [a SharePoint-riasztások kezelése, megtekintése vagy törlése](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) című témakört.

> [!NOTE]
> - Nem lehet riasztásokat küldeni terjesztési csoportnak. Csak a Security és az O365 csoportok támogatottak.
> - Az értesítési e-mail sablonok nem szabhatók testre. Ezek eléréséhez microsoft flow vagy SharePoint Designer munkafolyamatot kell használnia.
