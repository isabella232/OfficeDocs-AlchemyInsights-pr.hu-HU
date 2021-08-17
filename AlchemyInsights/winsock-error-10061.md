---
title: 1554-es nyertesek 10061-es hibakódja
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083232"
---
# <a name="winsock-error-10061"></a>A 10061-es hibakód

Ez a hibakód azt jelenti, hogy a Microsoft nem tudott TCP-szoftvercsatorna (kapcsolat) létesíteni a cél állomással. A hibát a legvalószínűbb oka a tűzfal konfigurációja okozza. A probléma megoldásához ellenőrizze az alábbi beállításokat:

- A tűzfal konfigurációjának ellenőrzése az URL-Microsoft 365 [IP-címtartományok adataival](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ha a hiba csak az Exchange Online Védelmi szolgáltatás (EOP) miatt jelenik meg, akkor korábban értesítést kellett volna kapni a levelezési [IP-címek Exchange Online Védelmi szolgáltatás változásokról.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Ellenőrizze, hogy az internetszolgáltató nem blokkolja-e a portot.

- Ellenőrizze az intelligens állomás és a célkiszolgáló beállításait az összekötőkben.

Vegye figyelembe Microsoft 365 hogy a bejövő kapcsolatok nem *tiltják* le ily módon.
