---
title: Naplózás kezelése
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524634"
---
# <a name="manage-journaling"></a><span data-ttu-id="5cc7b-102">Naplózás kezelése</span><span class="sxs-lookup"><span data-stu-id="5cc7b-102">Manage journaling</span></span>

<span data-ttu-id="5cc7b-103">A naplózás a bejövő és kimenő e-mail-kommunikáció rögzítésével segíthet a szervezetnek a jogi, szabályozási és szervezeti megfelelőségi követelmények teljesítésében.</span><span class="sxs-lookup"><span data-stu-id="5cc7b-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="5cc7b-104">Ne feledje:</span><span class="sxs-lookup"><span data-stu-id="5cc7b-104">Keep in mind:</span></span>

* <span data-ttu-id="5cc7b-105">A naplózás [kezelése](https://go.microsoft.com/fwlink/?linkid=2115259) előtt [](https://go.microsoft.com/fwlink/?linkid=2115469) szervezetkezelési és rekordkezelési engedélyekkel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="5cc7b-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="5cc7b-106">Be kell állítania egy naplópostafiókot, és (szükség esetén) be kell állítania egy másik naplópostafiókot.</span><span class="sxs-lookup"><span data-stu-id="5cc7b-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="5cc7b-107">További információt a Naplózás konfigurálása [az Exchange Online-ban című cikkben olvashat.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="5cc7b-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="5cc7b-108">Az Exchange Online-ban a létrehozható naplószabályok száma korlátozva van.</span><span class="sxs-lookup"><span data-stu-id="5cc7b-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="5cc7b-109">Részletes információkért lásd a Napló, az Átviteli és a Beérkezett üzenetek [szabálykorlátai című cikkeket.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="5cc7b-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="5cc7b-110">Az Exchange Online nem támogatja a naplójelentések Exchange Online-postaládákba való kézbesítését.</span><span class="sxs-lookup"><span data-stu-id="5cc7b-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="5cc7b-111">Naplópostafiókként meg kell adnia egy helyszíni archiválási rendszer vagy egy külső archiválási szolgáltatás e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="5cc7b-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
