---
title: A frissítések letöltésével, telepítésével és frissítésével kapcsolatos problémák Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9128"
- "9004429"
ms.openlocfilehash: 3db5fc4f2be0bbf845dec15b53f1299653f97ed75e12b04e8041de5982f5a74a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812821"
---
# <a name="fix-problems-with-the-download-installation-and-update-of-microsoft-edge"></a>A frissítések letöltésével, telepítésével és frissítésével kapcsolatos problémák Microsoft Edge

Mielőtt megkísérelné a javításokat, győződjön meg arról, hogy a számítógép operációs rendszer kompatibilis az Microsoft Edge rendszerrel, amely támogatja a Windows 10, 8, 8.1, 7 32 bites (x86) és 64 bites (x64) rendszert, valamint a macOS 10.12 Sierra és újabb verziókat. A fájlok letöltésével Microsoft Edge telepítésével és frissítésével kapcsolatos problémák megoldásához kövesse az alábbi utasításokat:

1. Ellenőrizze a hálózatot és a VPN-t:
    - Ellenőrizze a hálózati kapcsolatot.
    - A 403-as hiba azt sugallhatja, hogy a VPN blokkolja a letöltéseket. Bontsa a kapcsolatot a VPN-ről, és próbálkozzon újra a Microsoft Edge letöltésével.
1. Vegye officeapps.live.com a megbízható webhelyek listájára.
    Ha például az Internet Explorert használja az Microsoft Edge:
    1. Válassza **az Eszközök**  >  **Internetbeállítások lehetőséget.**
    2. A Biztonság **lapon** válassza a **Megbízható helyek**  >  **lehetőséget.**
    3. A **Webhely hozzáadása a zónához** területen írja be a , válassza a <https://officeapps.live.com> **Hozzáadás,** majd a Bezárás **lehetőséget.**
1. Újratelepítés Microsoft Edge: Windows számítógépen nem kell eltávolítania Microsoft Edge újratelepítése előtt. Az újratelepítés nincs hatással az előzményekre, a cookie-kra és a beállításokra sem.

    Mac gépen el kell távolítania Microsoft Edge újratelepítése előtt. Ezenkívül vissza kell állítania az előzményeket, a cookie-kat és a beállításokat.

    Az Microsoft Edge eltávolítása Macen:
    1. Nyissa meg a Findert.
    2. Az Alkalmazások **mappában** válassza **a** Microsoft Edge.
    3. Válassza **a Fájl** áthelyezése a  >  **kukába lehetőséget.**

    A következő Microsoft Edge újratelepítése Windows Mac számítógépen:
    1. Nyisson meg egy működő böngészőt.
    2. A böngésző letöltéséhez Microsoft Edge letöltési webhelyére.
1. Indítsa újra a számítógépet: Indítsa újra a számítógépet, és próbálja meg újratelepíteni Microsoft Edge.

