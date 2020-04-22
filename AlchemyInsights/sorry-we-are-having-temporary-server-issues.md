---
title: Az Office-alkalmazások javítása Elnézést, ideiglenes kiszolgálói problémák üzenettel kapcsolatosak
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764119"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Az Office-alkalmazások javítása "Sajnáljuk, ideiglenes kiszolgálóproblémák vannak" üzenet

Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és ellenőrizze, hogy azok nem akadályozzák-e az Office-alkalmazások internet-hozzáférését. Lásd [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Nyissa meg a**Futtatás** **indítása** > , majd írja be **a services.msc**. Győződjön meg arról, hogy a következő szolgáltatások futnak:
    - Hálózati csatlakoztatott eszközök automatikus beállítása
    - Hálózati lista szolgáltatás
    - Hálózati helyfigyelés
    - Windows eseménynapló

Ha a szolgáltatások egyike nem fut, próbálja meg elindítani. Ha problémája van a szolgáltatás elindításával, futtassa a következő parancsot egy emelt szintű engedélyekkel rendelkező parancssor megnyitásával:

**sfc /scannow**

A parancs befejezése után indítsa újra a számítógépet.

A részletes információt a ["Sajnáljuk, nem tudunk csatlakozni a fiókjához" című témakörben talál. Próbálkozzon később" hibaüzenet jelenik meg az aktiváláskor.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)