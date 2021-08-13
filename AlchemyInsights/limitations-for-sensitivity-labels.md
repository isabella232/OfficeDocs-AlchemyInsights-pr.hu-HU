---
title: A bizalmasság-címkék korlátozásai Office fájlokhoz SharePoint és OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813157"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>A bizalmasság-címkék korlátozásai Office fájlokhoz SharePoint és OneDrive

A bizalmasság-címkék engedélyezésekor Office a SharePoint és OneDrive, vegye figyelembe az alábbi követelményeket és korlátozásokat:

- SharePoint és a OneDrive nem tudja feldolgozni az asztali alkalmazásokból címkével és titkosítással címkével és titkosítással jelölt fájlokat, ha Office fájlok PowerQuery-adatokat, egyéni bővítmények által tárolt adatokat vagy egyéni XML-részeket tartalmaznak.
- SharePoint és OneDrive az Azure Information Protection (AIP) címkéivel már titkosított meglévő fájlokra ne alkalmazza automatikusan a bizalmasság-címkéket. Bizalmasság-címkék alkalmazása titkosított fájlokra: 
    - Győződjön meg arról, hogy áttelepített és közzétett AIP-címkéket a Microsoft 365 megfelelőségi központban.
    - Töltse le a címkével jelölt fájlokat, majd töltse fel őket az eredeti SharePoint vagy OneDrive helyre.
- Titkosított dokumentumok esetén a nyomtatás nem támogatott.

A korlátozásokról további információt a Bizalmasság-címkék engedélyezése Office fájlokhoz a SharePoint [és OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
