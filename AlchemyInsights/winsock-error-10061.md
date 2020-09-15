---
title: 1554 Winsock-hiba 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698864"
---
# <a name="winsock-error-10061"></a>WINSOCK-hiba 10061

Ez a hibakód azt jelzi, hogy a Microsoft nem tudott TCP-szoftvercsatornát (kapcsolatot) létesíteni a célállomással. A hiba legvalószínűbb oka a tűzfal-konfigurációval kapcsolatos probléma. A probléma megoldásához tekintse át a következő beállításokat:

- Tűzfal-konfiguráció ellenőrzése a [Microsoft 365 URL-címei és IP-címei](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) szerinti adatokkal

- Ha a hiba az Exchange Online védelmi szolgáltatással (EOP) függ, korábban értesítést kellett volna küldenie az [Exchange Online védelmi szolgáltatás IP-címeinek](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)módosításáról.

- Ellenőrizze, hogy az INTERNETSZOLGÁLTATÓja nem blokkolja-e a portot.

- Ellenőrizze az összekötők intelligens állomás-és célkiszolgáló-beállításait.

Fontos tudni, hogy a Microsoft 365 ilyen módon nem blokkolja a *bejövő* kapcsolatokat.
