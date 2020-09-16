---
title: Késések a SharePoint-és OneDrive-értesítések fogadásakor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727245"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Késések a SharePoint-és OneDrive-értesítések fogadásakor

- Először ellenőrizze a levélszemét vagy a Levélszemét mappát az e-mailben.
- Ha a **több fájlból vagy tárból érkező összes értesítés késik**, keresse fel a [szolgáltatás állapota irányítópultot](https://portal.office.com/adminportal/home?ref=/servicehealth) , és ellenőrizze, hogy vannak-e olyan tanácsadók/incidensek, amelyek a SharePoint vagy az Exchange alkalmazásban esetleg előfordulnak. Előfordulhat, hogy a probléma a SharePoint riasztási képességével vagy az e-mailek Exchange-ben való késésével jár. Azt is megtudhatja, hogy az egyéb e-maileket kézbesíti-e, és ha nem, a probléma valószínűleg az Exchange késésekkel jár.
- Ha **nincs kézbesítve egy adott fájl vagy tár egyéni figyelmeztetése**, próbálkozzon a törlésével és újbóli létrehozásával. A riasztás újbóli létrehozásához olvassa el a [SharePoint-értesítések kezelése, megtekintése és törlése](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) című témakört.

> [!NOTE]
> - Nem lehet értesítést küldeni a terjesztési csoportnak. Csak a biztonsági és O365-csoportok támogatottak.
> - A riasztási e-mail-sablonok nem szabhatók testre. Ezek eléréséhez a Microsoft flow vagy a SharePoint Designer munkafolyamatot kell használnia.
