---
title: Klasszikus SharePoint-naplójelentések
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741967"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>A SharePoint és a OneDrive naplózási naplói

## <a name="sharepoint-classic-audit-logs"></a>Klasszikus SharePoint-naplónaplók

Az SPO örökölt naplózása átlett telepítve az egyesített naplónaplóba (UAL). Az összes SPO örökölt naplózási jelentés most antól az UAL-n keresztül lesz, és az örökölt naplózási jelek átlettek telepítve az UAL-ba.

Legfontosabb változások:

* A vágás nem érhető el képességként.
* A naplózandó események kiválasztása NEM érhető el. Ebben a [dokumentumban](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) az alapértelmezés szerint elérhető naplózott események teljes listáját tartalmazza.
* A **Hely** beállítás a **Testreszabott jelentések** csoportban NEM érhető el.
* A **dokumentumok megnyitása vagy letöltése** események nem érhető el.

[Webhelycsoport naplózási beállításainak konfigurálása](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>A SharePoint és a OneDrive modern, egységes naplózási naplói a megfelelőségből

* [Az egyesített naplózás be- és kikapcsolása](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Nincs szükség további konfigurációra a SharePointban vagy a OneDrive-on belül.

A naplózási keresés sel ellenőrizheti a fájl(ok), a mappa(ok), a felhasználó(k), az engedélyek tevékenységét:

* [Fájl- és oldaltevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Mappatevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Megosztási és hozzáférési kérelmekkel kapcsolatos tevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Szinkronizálási tevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Webhely-adminisztrációs tevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Az események beolvasásáról a [Keresés a naplóban](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)című témakörben talál további információt.
