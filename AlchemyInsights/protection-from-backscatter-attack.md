---
title: Védelem a Backscatter-támadások ellen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036073"
---
# <a name="protection-from-backscatter-attack"></a>Védelem a Backscatter-támadások ellen

A Visszapattanópata az el nem küldött üzenetekről kapott nem kézbesítésről szóló jelentések (más néven a kézbesítésről szóló jelentések vagy visszapattanó üzenetek). A levélszemétküldők megfedik (hamisják) az üzeneteik **From:** címét, és gyakran valódi e-mail-címekkel adnak hitelességet az üzeneteikben. Ha tehát a levélszemétküldők elkerülhetetlenül küldenek üzeneteket nem létező címzetteknek, a cél levelezési kiszolgálót lényegében átveszi a rendszer arra, hogy kézbesíthetetlen üzenetet küldjenek vissza egy sikertelen kézbesítésről szóló jelentésből a **feladói** cím hamis feladójának.

További információt az [EOP Backscatter szolgáltatásában talál.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)

**A Visszakattoló elleni védelem engedélyezése**

A Backscatter-védelem engedélyezéséhez kövesse az alábbi lépéseket.

**protection.office.com > Threat Management > Policy > Antispam > Válassza a Levélszemétszűrő házirend és a Házirend szerkesztése > Levélszemét tulajdonságai > Megjelölés levélszemétként > sikertelen kézbesítésről szóló jelentés visszacsatoló levélszemétje > Beállítás "Be" beállításra**

Ha úgy véli, hogy feltörték a fiókját, tekintse át az alábbi információkat:

- [Válasz feltört e-mail-fiókra](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Letiltott felhasználók eltávolítása az Office 365 Korlátozott felhasználók portálján](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



