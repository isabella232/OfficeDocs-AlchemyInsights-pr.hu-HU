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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046754"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Az archív postaláda majdnem megtelt.

Ha a felhasználó figyelmeztetést kap; **Az archív postaláda majdnem** megtelt, vagy növelnie kell az archív postaládája méretét. Íme néhány tipp:

1. Ha a felhasználóhoz Exchange Online 1. csomag, frissítsen a **Exchange Online 2.** csomag licencre a méret 50 GB-osról 100 GB-ra való növeléséhez.
1. Ha a felhasználóhoz már hozzá van rendelve az alábbi lehetőségek valamelyike: **Exchange Online 2.** csomag vagy egy Exchange Online Exchange Online Archiválás bővítményt használó Exchange Online Archiválás 1. csomag, az alábbi lépésekkel engedélyezze az automatikus archiválást:
 
    1. [Csatlakozás Powershell Exchange Online át.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Futtassa az alábbi parancsmagot a felhasználó számára:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. A következő parancsmag futtatásával erősítse meg, hogy engedélyezve van a felhasználó számára:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

További információ:

- [Korlátlan archiválás engedélyezése – rendszergazdai súgó – Microsoft 365 megfelelőségi | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online korlátozások – A szolgáltatásleírások | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Frissítés másik vállalati csomagra | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

