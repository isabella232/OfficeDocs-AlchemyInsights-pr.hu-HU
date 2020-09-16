---
title: A Microsoft 365-alkalmazások kijavítása Sajnáljuk, mi ideiglenes kiszolgálói probléma jelenik meg
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758247"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>A Microsoft 365-alkalmazások rögzítése "Sajnáljuk, az ideiglenes kiszolgálói problémák merülnek fel" üzenet

Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfal, a víruskereső szoftverek és a proxybeállítások között, és győződjön meg arról, hogy a Microsoft 365-alkalmazásokban nem akadályozza meg az internet elérését. Lásd: [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Nyissa meg a **Start**  >  **Run**parancsot, és írja be a **Services. msc kifejezést**. Győződjön meg arról, hogy az alábbi szolgáltatások futnak:
    - Hálózati csatlakoztatott eszközök automatikus beállítása
    - Hálózati lista szolgáltatás
    - A hálózat helyének tudatosítása
    - Windows Eseménynapló

Ha az egyik szolgáltatás nem fut, próbálja meg elindítani. Ha probléma lép fel a szolgáltatás elindítása után, futtassa az alábbi parancsot az emelt szintű engedélyekkel rendelkező parancssor megnyitásával:

**sfc vizsgált**

A parancs befejezése után indítsa újra a számítógépet.

További információt az ["Sajnáljuk, nem lehet csatlakozni a fiókjához" című témakörben talál. Próbálkozzon újra később "hibaüzenet jelenik meg az aktiváláskor](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).