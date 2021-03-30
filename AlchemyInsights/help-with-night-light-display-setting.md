---
title: Segítség az éjszakai fény megjelenítési beállításával
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404663"
---
# <a name="help-with-the-night-light-display-setting"></a>Segítség az éjszakai fény megjelenítési beállításával

Az éjszakai megjelenítés beállításairól további információt A kijelző beállítása éjszakai megjelenítésre [Windows 10-ben.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Ha az éjszakai fény beállításai szürkén jelennek meg a Beállítások lapon, ellenőrizze a kijelző illesztőprogramját: 

1. Kattintson a tálcán a keresőmezőbe, írja  be az **Eszközkezelő** parancsot, majd a találatok között válassza az Eszközkezelő lehetőséget.
1. **Bontsa ki a videokártyákat.** 

Az éjszakai fény szolgáltatás sajnos nem érhető el, ha az eszköz DisplayLink illesztőprogramot vagy egyszerű kijelző-illesztőprogramot használ.

Az éjszakai fény funkció a legújabb grafikus technológiát használja, ezért előfordulhat, hogy frissítenie kell a kijelző illesztőprogramját:  

- A frissítéseket a **Start**  >  **Settings** Update & Windows Update Check for Updates  >    >  **(Biztonsági Windows**  >  **Update-frissítések** keresése) lapon ellenőrizheti.  

VAGY

- A hardver gyártójának támogatási webhelyén manuálisan töltse le és telepítse a legújabb illesztőprogramokat.

## <a name="reset-night-light-in-the-registry"></a>Éjszakai fény alaphelyzetbe állítása a beállításjegyzékben

Ha a képernyőillesztő frissítése nem működik, előfordulhat, hogy alaphelyzetbe kell állítania az éjszakai fényt a beállításjegyzékben.  

**Figyelem:** Ez a hibaelhárítási lépés csak haladó felhasználóknak ajánlott. Ha helytelenül módosítja a beállításjegyzéket, komoly problémák léphetnek fel. A további védelem érdekében a módosítás előtt biztonsági mentést kell a beállításjegyzékről, hogy probléma esetén visszaállítsa azt.

1. Írja be a **keresőmezőbe a regedit**, majd a találatok között **a** Beállításszerkesztő lehetőséget.

1. Ugrás a következő beállításkulcsra: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Exportálja, majd törölje a következő alkulcsot:$$windows.data.bluelightreduction.bluelightreductionstate

1. Exportálja, majd törölje a következő alkulcsot:$$windows.data.bluelightreduction.settings

1. Indítsa újra a Windowst, és ellenőrizze, hogy elérhetők-e az éjszakai fény beállításai.


