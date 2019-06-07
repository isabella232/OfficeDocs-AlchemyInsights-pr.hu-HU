---
title: A hozzáférés megtagadva üzenetet – problémamegoldás
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760343"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Üzenetek megtagadta a hozzáférést a Sharepoint/OneDrive Admin Center – problémamegoldás

Ha a hozzáférés megtagadásáról, tallózással keresse meg a Sharepoint/OneDrive Admin Center megkísérelte kap, győződjön meg arról, hogy [a felhasználó licenc hozzárendelése](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ha a felhasználói licenccel rendelkezik, akkor győződjön meg arról is [egy rendszergazda szerepkört](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , amelyhez hozzáférhet az admin-centers.

Ez a probléma akkor is előfordulhat, amikor a felhasználó törli, és újra létrehozza a ugyanolyan egyszerű felhasználónév (UPN). Az új fiók jön létre egy másik értéket PUID (Passport egyedi azonosító) segítségével. Ha a felhasználó megpróbál hozzáférni egy webhelycsoport vagy a OneDrive, a felhasználó rendelkezik egy helytelen PUID. A második forgatókönyv magában foglalja a könyvtár szinkronizálás az Active Directory szervezeti egységet (OU). Ha a felhasználó rendelkezik már bejelentkezett a SharePoint, majd átkerül egy másik szervezeti egység és SharePoint resynced, akkor ez a probléma tapasztalhatnak.

A probléma megoldásához a cikk [az Office 365 rendszerben a felhasználó visszaállítási](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)lépéseket az eredeti UPN kell visszaállítani.

Megjegyzés: Ha több felhasználónak, aki korábban a hozzáférést a OneDrive vagy a SharePoint felügyeleti központ nem érhető el, lehet egy ideiglenes szolgáltatást a probléma.  [Ellenőrizze a szolgáltatás egészségügyi irányítópult](https://portal.office.com/adminportal/home#/servicehealth).


