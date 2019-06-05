---
title: Teljesítmény problémák SharePoint- vagy OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719519"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>A SharePoint- vagy OneDrive lassú, nem elérhető vagy nem érhető el, ha több felhasználó

Több felhasználó, aki korábban az access OneDrive vagy a SharePoint webhely nem érhető el, ha a szolgáltatás átmeneti probléma lehet. [Ellenőrizze a szolgáltatás egészségügyi irányítópult](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Adjunk hozzá, és a felhasználói licenc

Győződjön meg arról, amikor a [felhasználók az Office 365 rendszerben üzleti licencek hozzárendelése](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Engedélyek hozzárendelése

Ha a felhasználó Sharepoint licencre van rendelve, és továbbra is a hozzáférés megtagadva üzenetet kap, ellenőrizze, hogy rendelkezik a [megfelelő jogosultsági szint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) hozzárendelt.

## <a name="consider-using-the-access-request-feature"></a>Fontolja meg a hozzáférési kérelem szolgáltatás

A [hozzáférési kérelem szolgáltatás](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) segítségével a felhasználók a tartalom megtekintéséhez engedéllyel jelenleg nem rendelkeznek hozzáférést kérni.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Lehetővé teszi egyéni parancsfájl hozzáférés megtagadva problémákat okozhat.

Vannak bizonyos helyzetek, ahol az *egyéni parancsfájlok engedélyezése* a szolgáltatás lehet tárni a hozzáférés megtagadva. Az érintett szolgáltatások listáját, biztonsági megfontolások és képessége, hogy tiltsa le a szolgáltatást. Látogasson el a [engedélyezése vagy tiltása egyéni parancsfájl](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

