---
title: Az archív postaláda majdnem megtelt.
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974405"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Az archív postaláda majdnem megtelt.

Ha a felhasználó figyelmeztetést kap; **Az archív postaláda majdnem megtelt,** vagy növelnie kell az archív postaládája méretét, íme néhány tipp:

1. Ha a felhasználóhoz Exchange Online 1. csomag van rendelve, frissítsen **az Exchange Online 2.** csomag licencére, és növelje a méretet 50 GB-ról 100 GB-ra.
1. Ha a felhasználóhoz már hozzárendelték az alábbi lehetőségek egyikét: **Exchange Online 2.** csomag vagy Exchange Online 1. csomag Exchange Online archiválási bővítő bővítővel, az alábbi lépésekkel engedélyezheti az automatikus archiválást:
 
    1. [Csatlakozás az Exchange Online Powershellhez.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Futtassa az alábbi parancsmagot a felhasználónak:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Az alábbi parancsmag futtatásával erősítse meg, hogy engedélyezve van a felhasználó számára:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

További információ:

- [ Korlátlan archiválás engedélyezése – rendszergazdai súgó – Microsoft 365 megfelelőségi | Microsoft Dokumentumok](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Az Exchange Online korlátai – Szolgáltatásleírások | Microsoft Dokumentumok](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Frissítés másik üzleti csomagra | Microsoft Dokumentumok](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

