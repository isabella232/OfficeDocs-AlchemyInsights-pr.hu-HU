---
title: Aktiválási probléma – Most nem lehet csatlakozni
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998155"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>A "Most nem lehet csatlakozni" üzenet Microsoft 365".

Ha megjelenik ez az üzenet, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy nem gátolja meg az Microsoft 365 hozzáférését. Lásd: [A Microsoft URL-címei és IP-címtartományai.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Válassza a **Start**  >  **Run ot,** majd írja be a **services.msc parancsot.** Győződjön meg arról, hogy az alábbi szolgáltatások mind futnak:
    - Hálózati eszközök automatikus beállítása
    - Hálózati lista szolgáltatás
    - Hálózati hely tájékoztatása
    - Windows Eseménynapló

Ha a szolgáltatások egyike nem fut, próbálja meg elindítani. Ha problémát okoz a szolgáltatás indítása, futtassa a következő parancsot egy magasabb szintű engedélyekkel rendelkező parancssor megnyitásával:

**sfc /scannow**

A parancs befejezését követően indítsa újra a számítógépet.

Részletes információkért lásd: "Sajnáljuk, nem lehet [csatlakozni a fiókjához. Kérjük, később](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)próbálkozzon újra" hibaüzenet jelenik meg, Office az Microsoft 365.