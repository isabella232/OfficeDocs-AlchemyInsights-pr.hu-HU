---
title: Klasszikus SharePoint-naplózási jelentések
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662210"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>A SharePoint és a OneDrive naplói

## <a name="sharepoint-classic-audit-logs"></a>Klasszikus SharePoint-napló

A Spongya örökölt naplózását az egyesített naplóba (UAL) migrálták. Mostantól az összes, a UAL-on keresztül megjelenő régi naplózási jelentés átkerül a UAL-ba.

Főbb változások:

* A körülvágás nem használható lehetőségként.
* A naplózandó események kiválasztása nem érhető el. Ebben a [dokumentumban](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) az alapértelmezés szerint elérhető naplózási események teljes listáját tekintheti meg.
* A **testre szabott jelentések** területen a **hely** lehetőség nem érhető el.
* A **dokumentumok megnyitása és letöltése** eseményekhez lehetőség nem érhető el.

[Webhelycsoport naplózási beállításainak megadása](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>A SharePoint és a OneDrive modern, egységes könyvvizsgálati naplók a megfelelőségi szolgáltatásból

* [Az egyesített naplózás be-és kikapcsolása](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

A SharePointban és az OneDrive-ban nincs szükség további konfigurálásra.

A naplózás naplózása szolgáltatással ellenőrizheti a fájl (ok), a mappa (ok), a felhasználó (k) és az engedélyek működését:

* [Fájlok és lapok tevékenysége](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Mappákkal kapcsolatos tevékenységek](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Megosztási és hozzáférés-kérési tevékenységek](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Szinkronizálási tevékenységek](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Webhely-felügyeleti tevékenységek](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Ha többet szeretne tudni az események beolvasásáról, olvassa el [a keresés a naplóban](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)című témakört.
