---
title: Intune-eszközök távoli felügyelete a TeamViewer segítségével
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555239"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Intune-eszközök távoli felügyelete a TeamViewer segítségével

Az Intune által kezelt eszközök távolról is feltekinthetők a [TeamViewer](https://www.teamviewer.com/)segítségével.

Ha az Intune-t a TeamViewer segítségével szeretné felügyelni, kövesse az alábbi lépéseket: 

Először szerezze be a TeamViewer hitelesítő adatait a TeamViewer Connector inIntune-n történő beállításához. Ez lehetővé teszi, hogy a rendszergazda adja meg a hitelesítő adatokat a TeamViewer Connector felhasználói felülete alatt Eszközök, egy egyszeri művelet létrehozása közötti kapcsolat Intune és a TeamViewer szolgáltatás.

**1. rész: Munkamenet indítása távoli eszközzel**

1. A **Minden eszköz csoportban**jelölje ki azt az eszközt, amelyhez távoli munkamenetet szeretne indítani.
2. From **... Több**, válassza **az Új távsegítség munkamenet lehetőséget.**
3. Válassza az **Igen** lehetőséget a távoli munkamenet létrehozásához.
    Miután a TeamViewer szolgáltatás nyugtázza az "Új távoli munkamenet indítása" kérést, az eszköz Áttekintés (vagy Essentials) ablaktáblájának részletei között megjelenik egy lehetőség a **távsegítség indítása.** Válassza **a Tovább lehetőséget** az ablaktábla kibontásához és a Távsegítség állapotának megjelenítéséhez.
4. Válassza **a Távoli munkamenet indítása** lehetőséget a munkamenet felügyeleti oldalon történő elindításához.
5. Válassza ki a TeamViewer bináris (Windows) letöltését, és válassza a **Futtatás**lehetőséget.<br/>
    **Megjegyzés:** A TeamViewer webhelyén megnyitott böngészőlapokat figyelmen kívül hagyhatja.

6. Nyugtázza a TeamViewer alkalmazás azon kérését, hogy módosítsa az eszközt (csak Windows rendszeren).
7. A TeamViewer alkalmazás elindul, és tartalmazza a munkamenet-kódot a kapcsolat hitelesítéséhez a távoli eszközzel.

**2. rész: A távoli munkamenetre szánt eszközön**

1. Nyissa meg az Intune vállalati portálját.
2. Keressen egy értesítési jelzőt: "A rendszergazda az eszköz vezérlését kéri egy távsegítség-munkamenethez", és válassza ki az értesítést.
3. Válassza ki a TeamViewer alkalmazás letöltését, vagy nyugtázza a TeamViewer alkalmazás letöltését az alkalmazásáruházból, és válassza a **Futtatás lehetőséget.**
    **Megjegyzés:** A TeamViewer webhelyén megnyitott böngészőlapokat figyelmen kívül hagyhatja.

4. Nyugtázza a TeamViewer alkalmazás azon kérését, hogy módosítsa az eszközt (csak Windows rendszeren).
5. A TeamViewer alkalmazás elindul, és tartalmazza a munkamenet-kódot a kapcsolat hitelesítéséhez a távoli eszközzel.
6. Egy felugró ablak megkérdezi, hogy engedélyezi-e a munkamenet indítását.

**Megjegyzés:** A TeamViewer szolgáltatás által létrehozott munkamenetkódok csak egyszeri használatra szolgálnak. Ha megszakad a kapcsolat, a következőket kell tennie:

1. Zárja be a TeamViewer alkalmazás példányát a távoli eszközön és a rendszergazdai munkaállomáson.
2. Zárja be a vállalati portált a távoli eszközön.
3. Új "Új távsegítség-munkamenet" kezdeményezése a felügyeleti portálról.
4. Nyissa meg újra a vállalati portált a távoli eszközön az új értesítés fogadásához.
5. Töltse le és nyissa meg a TeamViewer alkalmazást a távoli eszközön és a rendszergazdai munkaállomáson is, mint korábban.