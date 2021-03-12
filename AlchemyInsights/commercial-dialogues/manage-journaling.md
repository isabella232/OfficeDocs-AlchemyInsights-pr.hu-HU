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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745731"
---
# <a name="manage-journaling"></a><span data-ttu-id="7b284-102">Naplózás kezelése</span><span class="sxs-lookup"><span data-stu-id="7b284-102">Manage journaling</span></span>

<span data-ttu-id="7b284-103">A naplózás segítségével szervezete megválaszolhatja a jogi, szabályozási és szervezeti megfelelőségi követelményeket a bejövő és kimenő e-mail-kommunikáció rögzítésével.</span><span class="sxs-lookup"><span data-stu-id="7b284-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="7b284-104">Ne feledje:</span><span class="sxs-lookup"><span data-stu-id="7b284-104">Keep in mind:</span></span>

* <span data-ttu-id="7b284-105">A naplózás kezelése [előtt](https://go.microsoft.com/fwlink/?linkid=2115259) szervezetkezelési és rekordkezelési engedélyekkel kell rendelkeznie. [](https://go.microsoft.com/fwlink/?linkid=2115469)</span><span class="sxs-lookup"><span data-stu-id="7b284-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="7b284-106">Be kell állítania egy naplópostafiókot, és (ha szükséges) egy másik naplópostafiókot.</span><span class="sxs-lookup"><span data-stu-id="7b284-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="7b284-107">További információt a Naplózás beállítása [az Exchange Online-ban című cikkben olvashat.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="7b284-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="7b284-108">Az Exchange Online-ban a létrehozható naplószabályok száma korlátozva van.</span><span class="sxs-lookup"><span data-stu-id="7b284-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="7b284-109">Részletes információkért lásd: [Napló, átviteli és beérkezett üzenetekre vonatkozó szabályok korlátai.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="7b284-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="7b284-110">Az Exchange Online nem támogatja a naplójelentések Exchange Online-postaládába való kézbesítését.</span><span class="sxs-lookup"><span data-stu-id="7b284-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="7b284-111">A naplópostafiókként meg kell adnia egy helyszíni archiválási rendszer vagy egy külső archiválási szolgáltatás e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="7b284-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
