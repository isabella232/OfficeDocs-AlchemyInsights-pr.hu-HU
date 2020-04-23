---
title: A SharePoint riasztási értesítései nem kézbesítve
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742049"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>A SharePoint riasztási értesítései nem kézbesítve

Ellenőrizze az e-mailben található JUNK mappát, mivel néha figyelmeztetések jelenhetnek meg.

Határozza meg, hogy **az összes riasztás nem kézbesítve van-e,** vagy ha egy adott fájlból vagy tárból származó egyedi **riasztás** nem jelenik meg.

- **Egyéni riasztások nem kézbesítve:** Ha egy adott fájlból vagy tárból származó egyéni riasztás nem jelenik meg, megpróbálhatja törölni és újra létrehozni. A riasztás újbóli létrehozásához olvassa el A [SharePoint-értesítések kezelése, megtekintése és törlése](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) című témakört.
- **Az összes riasztás nem jelenik meg:** Ha több fájlvagy tárak összes riasztása nem jelenik meg, látogasson el a [Szolgáltatásállapot irányítópultjára,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) és ellenőrizze, hogy vannak-e olyan tanácsok/incidensek, amelyek a SharePoint vagy az Exchange programban előfordulhatnak. A probléma lehet a SharePoint riasztási képesség vagy késedelmek e-mailek az Exchange-en keresztül. Azt is fontos megjegyezni, hogy más e-mail kézbesítése folyamatban van-e, és ha nem, akkor a probléma valószínűleg az Exchange késedelmeivel kapcsolatos.

Gyakran feltett kérdések a riasztásokról:

- Nem lehet riasztásokat küldeni a terjesztési csoportnak, csak a biztonság és az O365 csoportok támogatottak.
- A figyelmeztető e-mail sablonok nem szabhatók testre; Ezek eléréséhez Microsoft FLOW vagy SharePoint Designer workflow szükséges.

További információ:

- **Riasztás beállítása**: A riasztások beállításáról a Riasztás [létrehozása értesítést kap, ha egy fájl vagy mappa megváltozik a SharePointban](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Riasztások elhárítása**: A riasztások hibaelhárításával kapcsolatos további információt a [Felhasználók nem kapnak SharePoint Online-riasztási értesítésekről.](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)
- **Speciális O365 megfelelőségi riasztási szabályzatok**: A riasztások beállításával kapcsolatos további tudnivalókért olvassa el a [Megfelelőségi riasztási szabályzatokat.](https://docs.microsoft.com/office365/securitycompliance/alert-policies)
- **SharePoint- és OneDrive-naplók**: Az események beolvasásáról a [Keresési naplóban](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)című témakörben talál további információt.
- **A komplex veszélyforrások elleni védelem által küldött riasztások**: A [SharePoint és a OneDrive ATP-jének](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)megtekintése.
- **Adatveszteség-megelőzési házirendek által küldött riasztások**: Lásd [a DLP-házirendek e-mail értesítéseit.](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)

## <a name="related-topics"></a>Kapcsolódó témakörök

Kiszeretné próbálni a Microsoft Flow-t a SharePoint Online-ban?

- [Folyamat létrehozása](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint és Folyamat](https://flow.microsoft.com//blog/sharepoint-and-flow/)
