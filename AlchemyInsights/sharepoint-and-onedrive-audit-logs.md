---
title: Klasszikus SharePoint-Naplójelentések
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068025"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint és OneDrive naplónapló

**SharePoint és OneDrive modern egyesített audit naplók a megfelelőségi**

- [Az egyesített Naplónaplózás be-és kikapcsolása](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Nincs szükség további konfigurálást a SharePoint vagy az OneDrive belül.

- A naplóvizsgálat kereséssel ellenőrizheti a fájl (ok), a mappa (ok), a felhasználó (k) és az engedélyek használatát.

    - [Fájl-és oldaltevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Mappatevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Kérésmegosztási és hozzáférési tevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Szinkronizálási tevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Webhely-adminisztrációs tevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- További információt az események lekéréséről [a naplózás keresése](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)című témakörben talál.

**Klasszikus SharePoint-naplófájlok**

Áttelepítette az SPO örökölt naplózását az egyesített Naplónaplóra (UAL). Ez lényegében azt jelenti, hogy minden SPO örökölt ellenőrzési jelentések most hajtott keresztül UAL, és a korábbi vizsgálati jelek átkerültek UAL.

Kulcs megváltozik:

- A kivágás mint képesség nem áll rendelkezésre.
- NEM érhető el az a szakasz, amelyben a naplózni kívánt eseményeket kiválasztja. Kérjük, olvassa el [ezt a dokumentumot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) az alapértelmezetten elérhető naplózott események teljes listájért.
- A **testreszabott jelentések** alatt lévő "hely" beállítás nem érhető el. 
- "Dokumentumok megnyitása vagy letöltése" események nem érhetők el. 

