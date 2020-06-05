---
title: A Microsoft 365-alkalmazások javítása Elnézést, ideiglenes kiszolgálói problémáküzenettel állunk
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582705"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>A Microsoft 365 alkalmazások javítása "Sajnáljuk, ideiglenes kiszolgálóproblémákkal kapcsolatos problémák vannak" üzenet

Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és ellenőrizze, hogy azok nem akadályozzák-e a Microsoft 365-alkalmazások internet-hozzáférését. Lásd [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Nyissa **Start**meg a  >  **Futtatás**indítása , majd írja be **a services.msc**. Győződjön meg arról, hogy a következő szolgáltatások futnak:
    - Hálózati csatlakoztatott eszközök automatikus beállítása
    - Hálózati lista szolgáltatás
    - Hálózati helyfigyelés
    - Windows eseménynapló

Ha a szolgáltatások egyike nem fut, próbálja meg elindítani. Ha problémája van a szolgáltatás elindításával, futtassa a következő parancsot egy emelt szintű engedélyekkel rendelkező parancssor megnyitásával:

**sfc /scannow**

A parancs befejezése után indítsa újra a számítógépet.

A részletes információt a ["Sajnáljuk, nem tudunk csatlakozni a fiókjához" című témakörben talál. Próbálkozzon később" hibaüzenet jelenik meg az aktiváláskor.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)