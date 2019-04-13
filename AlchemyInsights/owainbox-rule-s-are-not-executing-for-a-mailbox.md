---
title: 1332 OWA - Beérkezett üzenetek szabály(ok) nem végrehajtása postafiókhoz
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858746"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="4573c-102">A Beérkezett üzenetek szabály nem a várt módon működik</span><span class="sxs-lookup"><span data-stu-id="4573c-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="4573c-103">Ellenőrizze az alábbi beállításokat:</span><span class="sxs-lookup"><span data-stu-id="4573c-103">Verify the following settings:</span></span>

- <span data-ttu-id="4573c-104">Egy üzenet átirányíthatók, továbbított vagy automatikusan a Beérkezett üzenetekre vonatkozó szabályok alapján csak egy alkalommal a válaszok.</span><span class="sxs-lookup"><span data-stu-id="4573c-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="4573c-105">Átirányíthatja a legitim forrásból szabály (szabály a Beérkezett üzenetek vagy mail Attribútumfolyam-szabály, más néven átviteli szabály) legfeljebb tíz továbbítás címzett üzenetet adhat.</span><span class="sxs-lookup"><span data-stu-id="4573c-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="4573c-106">További tudnivalókért lásd: [napló, a szállítás, és a Beérkezett üzenetek szabály korlátai](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="4573c-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="4573c-107">A másodlagos naplózási postaláda Beérkezett üzenetekre vonatkozó szabályok nem működnek.</span><span class="sxs-lookup"><span data-stu-id="4573c-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="4573c-108">További információt az alternatív naplózási postaláda lásd: [alternatív naplózási postaláda](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="4573c-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="4573c-109">Ezek a problémák megoldásához, lásd: [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="4573c-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="4573c-110">A fenti hibákat nem alkalmazza, ha a Beérkezett üzenetek szabály diagnosztikai jelentés futtatása, mielőtt segítséget kér a probléma a Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="4573c-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="4573c-111">A postaláda megnyitása az Outlook alkalmazásban a weben, és kattintson a **Beállítások** \> **Beállítások** \> **Rendezés e-mail** \> **Beérkezett üzenetekre vonatkozó szabályok**.</span><span class="sxs-lookup"><span data-stu-id="4573c-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="4573c-112">A lap alján kattintson, **Ha a szabályok nem működnek a diagnosztikai jelentés létrehozásához kattintson ide**.</span><span class="sxs-lookup"><span data-stu-id="4573c-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
