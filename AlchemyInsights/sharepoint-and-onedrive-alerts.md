---
title: Nem kapja meg a SharePoint és az OneDrive riasztások
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/25/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 80423791ad558fc414d50608c73f823036432e14
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205529"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a>Nem kapja meg a SharePoint és az OneDrive riasztások

Először ellenőrizze az e-mailben található levélszemét vagy Levélszemét mappát.

Ezután állapítsa meg, hogy az **értesítések nem kerülnek kézbesítésekre** , vagy egy adott fájlból vagy könyvtárból származó **egyedi figyelmeztetést** nem kézbesíti a rendszer.

- Ha **nem kézbesíthető több fájl vagy tár figyelmeztetése**, látogasson el a [szolgáltatás egészségügyi irányítópultba](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) , és ellenőrizze, hogy vannak-e olyan figyelmeztetések/események, amelyek a SharePoint vagy az Exchange segítségével bekövetkezhetnek. A kérdés lehet a SharePoint riasztási képesség vagy késedelmek az e-maileket az Exchange. Is jegyzék vajon más elektronikus levél van lét kézbesített — ha nem, a kérdés van valószínű-val cserél késleltetés.
- Ha egy **adott fájlból vagy könyvtárból származó egyedi figyelmeztetést nem kézbesítünk**, próbáljuk meg törölni, majd újra létrehozni. A riasztás újbóli létrehozásához lásd: [SharePoint-riasztások kezelése, megtekintése vagy törlése](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0) .

> [!NOTE]
> - Terjesztési csoportnak nem lehet értesítéseket küldeni. Csak a biztonsági és O365 csoportok támogatottak.
> - A riasztási e-mail sablonok nem szabhatók testre. Ezeket a Microsoft flow vagy SharePoint Designer munkafolyamatot kell használnia.
