---
title: A jelzők nem működnek az Edge böngészőben
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676243"
---
# <a name="indicators-dont-work-using-edge-browser"></a>A jelzők nem működnek az Edge böngészőben

Miután létrehozott egy jelölőt, azt a Edge (Smartscreen) nem tudja tiszteletben hagyni. További információ: [Jelölők létrehozása IP-hez és URL-hez/tartományhoz.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1. lépés: Az alábbiak biztosítása

- Ellenőrizze, hogy helyes-e a jelölő (nem írja el az IP/URL-címet, helyes művelet, a megfelelő RBAC-csoportokat).
- Várjon legalább 2 órát a jelző létrehozása után, és vegye figyelembe a lehetséges késéseket.
- Győződjön meg arról, hogy a rendszer(eket) a Microsoft Defenderrel való, végpontként való végre útjára vannak véve.
- Ellenőrizze, hogy a rendszerek képesek-e kommunikálni a felhővel.
- Ellenőrizze, hogy a Smartscreen engedélyezve van-e, és elérhető-e a [tesztwebhelyen.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>2. lépés: A potenciális probléma megoldása

- Győződjön meg arról, hogy az ügyfél megfelel a követelményeknek. Részletes információkért lásd: [Jelölők létrehozása IP-hez és URL-hez/tartományhoz.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Győződjön meg arról, hogy az Edge böngésző legújabb verzióját használja. A legújabb verzióra a Következő verziójú Microsoft Edge [talál.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Indítsa újra a Microsoft Edge böngészőt.
- Nyissa meg azt a webhelyet, amelyhez beállításjelzőt adott meg. Ha a webhely nem a várt módon jelenik meg, folytassa a 3. lépéssel. 

## <a name="step-3-collect-data"></a>3. lépés: Adatgyűjtés

- Gyűjtse **össze az MDEClientAnalyzer** diagnosztikai adatokat. Utasításokért lásd: [A számítógépeket a Microsoft Defender végpontra való be- vagy kitöltőgépekkel kapcsolatos problémák.](issues-with-onboarding-machines.md)
- Ha már jól tudja telepíteni és gyűjteni a Fiddler-nyomkövetést, tekintse meg a [Telerik Fiddler (Telerik Fiddler) adatokat.](http://www.telerik.com/fiddler)
- Ha a Microsoft ügyfélszolgálatának útmutatását részesíti előnyben, válassza az alábbi Támogatás ikont egy támogatási eset megnyitásához.
