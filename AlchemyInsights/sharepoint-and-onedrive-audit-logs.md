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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992620"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint és OneDrive naplónapló

## <a name="sharepoint-classic-audit-logs"></a>Klasszikus SharePoint-naplófájlok

Az SPO örökölt naplózását az egyesített Naplónaplóba telepítették át. Minden SPO örökölt ellenőrzési jelentések most hajtott keresztül UAL, és a korábbi vizsgálati jelek kerültek át a UAL.

Kulcs megváltozik:

* A tisztítás nem áll rendelkezésre.
* A naplózni kívánt események nem érhetők el. A [dokumentum](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) alapértelmezés szerint elérhető naplózott eseményeinek teljes listáját olvassa el.
* A **testreszabott jelentések** alatt lévő **helybeállítás** nem érhető el.
* A **megnyitási vagy letöltési dokumentum** események opció nem érhető el.

[Helycsoport naplózási beállításainak konfigurálása](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint és OneDrive modern egyesített audit naplók a megfelelőségi

* [Az egyesített Naplónaplózás be-és kikapcsolása](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Nincs szükség további konfigurálást a SharePoint vagy az OneDrive belül.

A naplóvizsgálat kereséssel ellenőrizheti a fájl (ok), a mappa (ok), a felhasználó (k) és az engedélyek használatát.

* [Fájl-és oldaltevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Mappatevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Kérésmegosztási és hozzáférési tevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Szinkronizálási tevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Webhely-adminisztrációs tevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

További információt az események lekéréséről [a naplózás keresése](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)című témakörben talál.
