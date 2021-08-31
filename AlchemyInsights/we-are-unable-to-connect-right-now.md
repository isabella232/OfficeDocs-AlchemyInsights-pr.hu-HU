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
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744597"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>A "Jelenleg nem lehet csatlakozni" hibaüzenet Microsoft 365".

Megjegyzés: Ha az Windows régebbi verzióját használja (például Windows 7 SP1 vagy Windows Server 2008 R2), [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) az egyszerű javítás használatával engedélyezze alapértelmezés szerint a TLS 1.2-t. További információt a Frissítés a [TLS 1.1 és a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)alapértelmezett biztonságos protokollként való engedélyezéséhez a Windowsbanhttps://Windows.

Ha megjelenik ez az üzenet, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy nem gátolja meg az Microsoft 365 hozzáférését. Lásd: [A Microsoft URL-címei és IP-címtartományai.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Válassza a **Start**  >  **Run ot,** majd írja be a **services.msc parancsot.** Győződjön meg arról, hogy az alábbi szolgáltatások mind futnak:
    - Hálózati eszközök automatikus beállítása
    - Hálózati lista szolgáltatás
    - Hálózati hely tájékoztatása
    - Windows Eseménynapló

Ha a fenti szolgáltatások egyike nem fut, próbálja meg elindítani. Ha problémát okoz a szolgáltatás indítása, futtassa a következő parancsot egy magasabb szintű engedélyekkel rendelkező parancssor megnyitásával:

**sfc /scannow**

A parancs befejezését követően indítsa újra a számítógépet.

Részletes információkért lásd: "Sajnáljuk, nem lehet [csatlakozni a fiókjához. Kérjük, próbálkozzon](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)újra később" hibaüzenet jelenik meg, Office a Microsoft 365.