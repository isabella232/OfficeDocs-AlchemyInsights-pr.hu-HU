---
title: 1554 Winsock hiba 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766171"
---
# <a name="winsock-error-10061"></a>Winsock hiba 10061

Ez a hibakód azt jelenti, hogy a Microsoft nem tudott TCP-szoftvercsatornát (kapcsolatot) létrehozni a célállomással. A hiba legvalószínűbb oka a tűzfal konfigurációjának hibája. A probléma megoldásához ellenőrizze az alábbi beállításokat:

- A tűzfal konfigurációjának ellenőrzése a [Microsoft 365 URL-címeiben és IP-címtartományaiban](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) szereplő adatokkal

- Ha a hiba az Exchange Online Protection (EOP) hibájára vonatkozik, korábban értesítenie kellett volna az [Exchange Online Protection IP-címeinek módosításáról.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Ellenőrizze, hogy az internetszolgáltató (ISP) nem blokkolja-e a portot.

- Ellenőrizze az intelligens állomás- és célkiszolgáló beállításait az összekötőkben.

Ne feledje, hogy a Microsoft 365 nem blokkolja a *bejövő* kapcsolatokat ilyen módon.
