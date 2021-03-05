---
title: A MIM-szinkronizálási szolgáltatás konfigurálása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481873"
---
# <a name="configure-mim-sync-service"></a>A MIM-szinkronizálási szolgáltatás konfigurálása

A Microsoft Identity Manager (MIM) szinkronizálási szolgáltatás a MIM összetevője. Ez egy központosított helyszíni szolgáltatás, amely információkat tárol és integrál a több helyszíni könyvtárakkal és adatbázisokkal rendelkező szervezetek számára. A MIM-szinkronizálással kapcsolatos problémát akkor lehet megoldani, ha a problémát egy nemrég frissülő mim-frissítésben javította, vagy ha az alábbi szakaszban említett egyéb problémák egyike.

**Ajánlott lépések**

1. Győződjön meg arról, hogy a MIM Sync legújabb frissítését használja, és ellenőrizze a [MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) kibocsátási megjegyzéseit annak megállapításához, hogy a probléma megoldódott-e egy frissítésben.
2. Ha a probléma az Általános LDAP, az Generic SQL, a Lotus Domino vagy a Web Services összekötővel kapcsolatos, győződjön meg arról, hogy az általános összekötők legújabb frissítését [használja.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Ha egy MIM-szinkronizálási futtatása hibát jelez, [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) a lehetséges okok meghatározásához tekintse meg a futtatás hibakódokat táblázatát.
4. Ha a futtatás a **extension-dll-exception** kiterjesztéssel leáll, akkor a szavakra kattintva nyissa meg az **Összekötő** térobjektum tulajdonságablakát, és kattintson a Stack Trace **gombra,** hogy további információt látsson a mögöttes okról, az [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)leírásának megfelelő módon.
5. Ha a PCNS összetevő a **6025-ös** hibát jelenti az eseménynaplóban a jelszó-szinkronizálás során, az útmutatóban ellenőrizheti a [PCNS 6025-ös](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)hibajelentési hibáinak elhárítását.
6. Ha lassú a teljes szinkronizálás a FIM  szolgáltatáskezelő ügynökkel, ellenőrizze a TempDB automatikus növekvő beállítását, a lassú szinkronizálás vagy a teljes szinkronizálás lelassulása – hibaelhárítási [leírásnak megfelelő módon.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. Ha a FIM szolgáltatáskezelő ügynökével sikertelen létrehozású webszolgáltatások esetén a leállított kiszolgáló hibát talál, az okokat áttekintheti a támogatási információk [között:](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) sikertelen létrehozás-létrehozás webszolgáltatásokon keresztül.

