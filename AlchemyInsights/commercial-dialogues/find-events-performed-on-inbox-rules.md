---
title: A beérkezett üzenetekre vonatkozó szabályokon végrehajtott események megkeresése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482597"
---
# <a name="find-events-performed-on-inbox-rules"></a>A beérkezett üzenetekre vonatkozó szabályokon végrehajtott események megkeresése

A beérkezett üzenetekre vonatkozó szabályok létrehozásakor, megváltoztatva vagy törlésekor a napló rögzíti az eseményeket. A következőt kell áttekintenünk:

1. Menjen az [Office 365 Biztonsági & megfelelőségi központba.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Válassza a > naplókeresés lehetőséget.

    > [!NOTE]
    > Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, akkor most kapcsolja be. Ha ez a funkció nincs bekapcsolva, a keresési eredmények nem fogják tudni lekeresni az előző dátumok adatait.
1. Jelölje ki a Tevékenységek mezőt, és keresse meg az Exchange-postaláda-tevékenységeket, majd New-InboxRule Levelezési szabály létrehozása az Outlook Web Appból lehetőséget. Amikor végzett, kattintson az ablakon kívülre a Tevékenységek ablaktábla kis méretűvé állításhoz.
1. Adja meg a dátumtartományt, majd a Felhasználók mezőben válassza ki a vizsgálni kívánt felhasználó felhasználónevét. Egyszerre több felhasználót is kijelölhet.
1. Válassza a Keresés lehetőséget. A tevékenységek az Eredmények alatt jelennek meg.
1. A részletek megtekintéséhez jelöljön ki egy tevékenységet, majd válassza a További információ lehetőséget. A Paraméterek szakaszban láthatja a szabály nevét, a beállított feltételeket és a szabály által meghozott műveleteket.

További információ: Keresés az Office 365 naplójában a gyakori esetek elhárításához.