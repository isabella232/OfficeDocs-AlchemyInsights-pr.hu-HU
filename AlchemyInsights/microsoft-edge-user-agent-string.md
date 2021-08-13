---
title: Microsoft Edge ügynök karakterláncának megjelenítése (asztal)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: 9311f17298fff3fee3282fe05bd1ddcd02780a80097e86b29d56ffd575a9a571
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976003"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a>Microsoft Edge ügynök karakterláncának megjelenítése (asztal)

Felhasználói ügynök (UA) karakterláncok segítségével lehet észlelni, hogy egy adott böngésző melyik verzióját használják egy adott operációs rendszeren. Más böngészőkhöz Microsoft Edge információk a "Felhasználói ügynök" HTTP-fejlécen adatokat tartalmaznak minden alkalommal, amikor egy webhelyre vonatkozó kérést tesz. A böngészőverzióra vonatkozó információk a JavaScripten keresztül is elérhetők a "navigator.userAgent" érték lekérdezésével.

Azt javasoljuk, hogy a webfejlesztők akkor használják a funkcióészlelést, amikor csak lehetséges, hogy javítsák a kódhasználatot, csökkentsék a kód töredelhetőségét, és kiküszöbölzék a kódtörés kockázatát az UA karakterlánc jövőbeli frissítései esetén.

További információt a Felhasználói ügynök [karakterláncának Microsoft Edge (asztali) oldalon.](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)