---
title: Nem kézbesítve a SharePoint riasztási értesítései
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
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751245"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Nem kézbesítve a SharePoint riasztási értesítései

Jelölje be az e-mailek levélszemét mappáját, mert időnként riasztások is előfordulhatnak.

Annak megállapítása, hogy az **összes értesítés nem kézbesítve** van-e, illetve hogy nem kézbesíti-e az adott fájl vagy tár **Egyéni figyelmeztetését** .

- A **rendszer nem kézbesíti az egyes riasztásokat**: Ha egy adott fájlból vagy tárból érkező egyéni figyelmeztetést nem kézbesítenek, akkor megkísérelheti törölni és újból létrehozni azt. A riasztás újbóli létrehozásához olvassa el a [SharePoint-értesítések kezelése, megtekintése és törlése](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) című témakört.
- A rendszer **nem kézbesíti az összes értesítést**: Ha a több fájlból vagy tárból származó összes értesítés nem érhető el, keresse fel a [szolgáltatás állapota irányítópultot](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , és ellenőrizze, hogy vannak-e olyan tanácsadók/incidensek, amelyek a SharePoint vagy az Exchange alkalmazásban esetleg előfordulnak. A probléma lehet a SharePoint riasztási képessége vagy az e-mailek késése az Exchange-ben. Fontos tudni, hogy más e-maileket kézbesítenek-e, és ha nem, a probléma valószínűleg az Exchange késésekkel fog rendelkezni.

Gyakori kérdések az értesítésekről:

- Nem lehet értesítéseket küldeni a terjesztési csoportnak, csak a biztonsági és O365-csoportok támogatottak.
- A riasztási e-mail-sablonok nem szabhatók testre; Ezek eléréséhez Microsoft FLOW vagy SharePoint Designer-munkafolyamatot kell használnia.

## <a name="related-topics"></a>Kapcsolódó témakörök

Szeretné kipróbálni a Microsoft flow-t a SharePoint Online-ban?

- [Folyamatábra létrehozása](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint és flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
