---
title: Az Office-alkalmazások rögzítése sajnálom, mi van az ideiglenes kiszolgáló kérdések üzenet
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627992"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Az Office-alkalmazások kijavítása "sajnálom, mi van az ideiglenes szerver kérdések" üzenet

Ha ezt az üzenetet kapja, próbálkozzon a következőkkel:

1. Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy azok nem akadályozzák az Office alkalmazásokhoz való internet-hozzáférést. Lásd [az Office 365 URL-címeket és IP-címtartományokat](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Megy **elkezd** > **fuss**, aztán típus **Services. msc**. Ellenőrizze, hogy a következő szolgáltatások futnak-e:
    - Hálózati csatlakoztatott eszközök automatikus telepítése
    - Hálózatilista-szolgáltatás
    - Hálózati helyfigyelés
    - Windows eseménynaplójában

Ha az egyik ilyen szolgáltatás nem fut, próbálja meg elindítani. Ha problémája van a szolgáltatás elindításával, futtassa a következő parancsot egy emelt szintű engedélyekkel rendelkező parancssorablak megnyitásával:

**sfc vizsgált**

A parancs befejeződése után indítsa újra a számítógépet.

Részletes információkért lásd: ["bocsánat, nem tudunk kapcsolódni a fiókjához. Próbálkozzon később, amikor aktiválja az Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).