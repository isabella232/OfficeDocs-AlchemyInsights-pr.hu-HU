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
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="0fded-102">Az archív postaláda majdnem megtelt.</span><span class="sxs-lookup"><span data-stu-id="0fded-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="0fded-103">Ha a felhasználó figyelmeztetést kap; **Az archív postaláda majdnem megtelt,** vagy növelnie kell az archív postaládája méretét, íme néhány tipp:</span><span class="sxs-lookup"><span data-stu-id="0fded-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="0fded-104">Ha a felhasználóhoz Exchange Online 1. csomag van rendelve, frissítsen **az Exchange Online 2.** csomag licencére, és növelje a méretet 50 GB-ról 100 GB-ra.</span><span class="sxs-lookup"><span data-stu-id="0fded-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="0fded-105">Ha a felhasználóhoz már hozzárendelték az alábbi lehetőségek egyikét: **Exchange Online 2.** csomag vagy Exchange Online 1. csomag Exchange Online archiválási bővítő bővítővel, az alábbi lépésekkel engedélyezheti az automatikus archiválást:</span><span class="sxs-lookup"><span data-stu-id="0fded-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="0fded-106">[Csatlakozás az Exchange Online Powershellhez.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="0fded-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="0fded-107">Futtassa az alábbi parancsmagot a felhasználónak:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="0fded-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="0fded-108">Az alábbi parancsmag futtatásával erősítse meg, hogy engedélyezve van a felhasználó számára:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="0fded-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="0fded-109">További információ:</span><span class="sxs-lookup"><span data-stu-id="0fded-109">For more information see:</span></span>

- [<span data-ttu-id="0fded-110"> Korlátlan archiválás engedélyezése – rendszergazdai súgó – Microsoft 365 megfelelőségi | Microsoft Dokumentumok</span><span class="sxs-lookup"><span data-stu-id="0fded-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="0fded-111">Az Exchange Online korlátai – Szolgáltatásleírások | Microsoft Dokumentumok</span><span class="sxs-lookup"><span data-stu-id="0fded-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="0fded-112">Frissítés másik üzleti csomagra | Microsoft Dokumentumok</span><span class="sxs-lookup"><span data-stu-id="0fded-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

