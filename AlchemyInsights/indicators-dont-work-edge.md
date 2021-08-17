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
ms.openlocfilehash: ff7a2ee4c97c579422c7679c461f6fb288a9235ff9056be1c56e80b1d6379723
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887442"
---
# <a name="indicators-dont-work-using-edge-browser"></a>A jelzők nem működnek az Edge böngészőben

Miután létrehozott egy jelölőt, azt a Edge (Smartscreen) nem tudja tiszteletben hagyni. További információ: [Jelölők létrehozása IP-hez és URL-hez/tartományhoz.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1. lépés: Az alábbiak biztosítása

- Ellenőrizze, hogy helyes-e a jelölő (nem írja el az IP/URL-címet, helyes művelet, a megfelelő RBAC-csoportokat).
- Várjon legalább 2 órát a jelző létrehozása után, és vegye figyelembe a lehetséges késéseket.
- Győződjön meg arról, hogy a rendszer(eket) a Microsoft Defenderrel való, végpontként való végre útjára vannak véve.
- Ellenőrizze, hogy a rendszerek képesek-e kommunikálni a felhővel.
- Ellenőrizze, hogy a Smartscreen engedélyezve van-e, és elérhető-e a [tesztwebhelyen.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>2. lépés: A potenciális probléma megoldása

- Győződjön meg arról, hogy az ügyfél megfelel a követelményeknek. Részletes információkért lásd: [Jelölők létrehozása IP-hez és URL-hez/tartományhoz.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Győződjön meg arról, hogy az Edge böngésző legújabb verzióját használja. A legújabb verzióra a Következő verziójú Microsoft Edge [talál.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Indítsa újra a Microsoft Edge böngészőt.
- Nyissa meg azt a webhelyet, amelyhez beállításjelzőt adott meg. Ha a webhely nem a várt módon jelenik meg, folytassa a 3. lépéssel. 

## <a name="step-3-collect-data"></a>3. lépés: Adatgyűjtés

- Gyűjtse **össze az MDEClientAnalyzer** diagnosztikai adatokat. Utasításokért lásd: [A számítógépeket a Microsoft Defender végpontra való be- vagy kitöltőgépekkel kapcsolatos problémák.](issues-with-onboarding-machines.md)
- Ha jól érzi magát a Fiddler-nyomkövetés telepítésében és összegyűjtésében, tekintse meg a [Telerik Fiddler (Telerik Fiddler) adatokat.](http://www.telerik.com/fiddler)
- Ha a Microsoft ügyfélszolgálatának útmutatását részesíti előnyben, válassza az alábbi Támogatás ikont egy támogatási eset megnyitásához.
