---
title: Aktiválási probléma – jelenleg nem tudunk csatlakozni
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725985"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>A Microsoft 365-alkalmazások rögzítése "a kapcsolat most nem érhető el" üzenet

Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfal, a víruskereső szoftverek és a proxybeállítások között, és győződjön meg arról, hogy a Microsoft 365-alkalmazásokban nem akadályozza meg az internet elérését. Lásd: [Microsoft URL-EK és IP-](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)címtartományok.

2. Nyissa meg a **Start**  >  **Run**parancsot, és írja be a **Services. msc kifejezést**. Győződjön meg arról, hogy az alábbi szolgáltatások futnak:
    - Hálózati csatlakoztatott eszközök automatikus beállítása
    - Hálózati lista szolgáltatás
    - A hálózat helyének tudatosítása
    - Windows Eseménynapló

Ha az egyik szolgáltatás nem fut, próbálja meg elindítani. Ha probléma lép fel a szolgáltatás elindítása után, futtassa az alábbi parancsot az emelt szintű engedélyekkel rendelkező parancssor megnyitásával:

**sfc vizsgált**

A parancs befejezése után indítsa újra a számítógépet.

További információt az ["Sajnáljuk, nem lehet csatlakozni a fiókjához" című témakörben talál. Próbálkozzon újra később "hibaüzenet jelenik meg, amikor aktiválja az Office-t a Microsoft 365-ből](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).