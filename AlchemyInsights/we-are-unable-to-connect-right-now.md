---
title: Aktiválási probléma - Jelenleg nem tudunk csatlakozni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716174"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Az Office-alkalmazások javítása "Jelenleg nem tudunk csatlakozni" üzenet

Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és ellenőrizze, hogy azok nem akadályozzák-e az Office-alkalmazások internet-hozzáférését. Lásd: [Microsoft URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Nyissa meg a**Futtatás** **indítása** > , majd írja be **a services.msc**. Győződjön meg arról, hogy a következő szolgáltatások futnak:
    - Hálózati csatlakoztatott eszközök automatikus beállítása
    - Hálózati lista szolgáltatás
    - Hálózati helyfigyelés
    - Windows eseménynapló

Ha a szolgáltatások egyike nem fut, próbálja meg elindítani. Ha problémája van a szolgáltatás elindításával, futtassa a következő parancsot egy emelt szintű engedélyekkel rendelkező parancssor megnyitásával:

**sfc /scannow**

A parancs befejezése után indítsa újra a számítógépet.

A részletes információt a ["Sajnáljuk, nem tudunk csatlakozni a fiókjához" című témakörben talál. Próbálkozzon később" hibaüzenet jelenik meg, amikor aktiválja az Office-t a Microsoft 365-ből.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)