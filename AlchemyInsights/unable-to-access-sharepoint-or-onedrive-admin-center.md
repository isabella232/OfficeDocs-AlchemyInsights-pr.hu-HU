---
title: Nem lehet elérni SharePoint felügyeleti OneDrive-et
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020446"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Nem lehet elérni SharePoint felügyeleti OneDrive-et

- Ha az SharePoint vagy OneDrive Felügyeleti központ webhelye nem érhető el vagy nem érhető el, átmeneti szolgáltatáshibát okozhat, amely miatt SharePoint felhasználók időnként késéseket vagy navigációs hibákat tapasztalhatnak OneDrive-tartalmak elérésekor. Ellenőrizze a [Szolgáltatás állapota irányítópulton,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) hogy nincs-e hatással a szervezete.

- A globális és a SharePoint-rendszergazdákhoz hozzá kell rendelni egy SharePoint-licencet. Az újonnan létrehozott fiókok esetén, amelyekhez éppen hozzárendelt egy SharePoint-licencet vagy rendszergazdai szerepkört, a SharePoint elérésekor hibaüzenet, például a „hozzáférés megtagadva” vagy a „felhasználó nem található” jelenik meg. Adjon legalább 24 órát a szinkronizálás számára, hogy végbemenjen a rendszereink között. Megértjük, hogy a 24 óra hosszú időnek tűnhet. Sok esetben már dolgozunk a megoldáson.

- Privileged Identity Management ([PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)felhasználói akkor kaphatnak hozzáférést megtagadva, ha a hozzáférési időkeret nagyon kicsi. Lásd: Hozzáférés megtagadva [a PIM-fiókokhoz.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)