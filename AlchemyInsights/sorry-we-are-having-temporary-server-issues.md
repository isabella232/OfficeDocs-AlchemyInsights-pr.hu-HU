---
title: A Microsoft 365-ös appok kijavítása Sajnáljuk, átmeneti kiszolgáló-problémákról következő üzenet jelenik meg
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835273"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>A Microsoft 365-alkalmazások "Sajnáljuk, ideiglenes kiszolgáló-problémákat tudunk" üzenetének kijavítása

Ha megjelenik ez az üzenet, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy nem gátolja meg a Microsoft 365-alkalmazásokhoz való internet-hozzáférést. Lásd: [URL-ek és IP-címtartományok.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Válassza a **Start**  >  **Run ot,** majd írja be a **services.msc parancsot.** Győződjön meg arról, hogy az alábbi szolgáltatások mind futnak:
    - Hálózati eszközök automatikus beállítása
    - Hálózati lista szolgáltatás
    - Hálózati hely tájékoztatása
    - Windows eseménynapló

Ha a szolgáltatások egyike nem fut, próbálja meg elindítani. Ha problémát okoz a szolgáltatás indítása, futtassa a következő parancsot egy magasabb szintű engedélyekkel rendelkező parancssor megnyitásával:

**sfc /scannow**

A parancs befejezését követően indítsa újra a számítógépet.

Részletes információkért lásd: "Sajnáljuk, nem lehet [csatlakozni a fiókjához. Kérjük, próbálkozzon újra később" hibaüzenet jelenik meg az aktiváláskor.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)