---
title: SharePoint értesítések nem kézbesítése
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 05bd913098372a57d3061e8c516a6a6b4f0a9bdafde02acc930062d6281d06dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957903"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint értesítések nem kézbesítése

Ellenőrizze a Levélszemét mappát az e-mailjeiben, mert néha előfordulhat, hogy ott is riasztják a riasztásokat.

Állapítsa **meg, hogy nem történik-e** meg az összes riasztás kézbesítése, vagy egy adott fájlból vagy tárból származó egyes riasztások nem. 

- **Az egyes értesítések kézbesítése** nem történik meg: Ha egy adott fájlból vagy tárból származó különálló riasztás nem lesz kézbesítve, megpróbálhatja törölni, majd ismét létrehozni. Az értesítések újbóli megtekintéséhez tekintse [meg, tekintse SharePoint vagy](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) törölje az értesítéseket.
- **Nem történik** meg minden riasztás kézbesítése: Ha több fájlból vagy [](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) tárból nem kap meg minden riasztást, a Szolgáltatás állapota irányítópulton ellenőrizze, hogy nincsenek-e az adott fájlokkal vagy tárakkal kapcsolatban esetlegesen előforduló SharePoint vagy Exchange. A problémát az e-mailek SharePoint vagy késése okozhatja a Exchange. Azt is fontos megjegyezni, hogy más e-mailek kézbesítése történik-e, és ha nem, akkor a probléma valószínűleg Exchange késéssel.

Gyakori kérdések a riasztásokkal kapcsolatban:

- Nem lehet riasztásokat küldeni a terjesztési csoportoknak, csak a biztonsági és az O365-csoportok támogatottak.
- Az értesítő e-mail sablonok nem szabhatók testre; ezek eléréséhez a Microsoft FLOW vagy a SharePoint Designer-munkafolyamatot kell használnia.

## <a name="related-topics"></a>Kapcsolódó témakörök

Szeretné kipróbálni az Microsoft Flow az SharePoint-ban?

- [Új Flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint és Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
