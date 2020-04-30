---
title: DLP használata az átviteli szabályokban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915182"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="b2d05-102">DLP használata az átviteli szabályokban</span><span class="sxs-lookup"><span data-stu-id="b2d05-102">Using DLP in transport rules</span></span>

<span data-ttu-id="b2d05-103">Az adatveszteség-megelőzés (DLP) meglévő átvitelbe való integrálásához használja a következő feltételt: „\*\* Ha az üzenet tartalmaz... Bizalmas adatokat\*\*“ az Átviteli szabály beállításaiban.</span><span class="sxs-lookup"><span data-stu-id="b2d05-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="b2d05-104">**További részletek:**</span><span class="sxs-lookup"><span data-stu-id="b2d05-104">**For more details, see:**</span></span>

- <span data-ttu-id="b2d05-105">Integrált DLP-bizalmasadat-típusok az átviteli szabályokban: [Bizalmas információkra vonatkozó szabályok integrálása](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="b2d05-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="b2d05-106">Emellett a szabályt házirendteszttel vagy anélkül is tesztelheti a szabály Tesztelési módjának használatával.</span><span class="sxs-lookup"><span data-stu-id="b2d05-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="b2d05-107">Tesztelés előtt várnia kell 30 percet a szabály létrehozása után.</span><span class="sxs-lookup"><span data-stu-id="b2d05-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="b2d05-108">Lásd: [E-mail forgalmi/Átviteli szabályok tesztelése](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="b2d05-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="b2d05-109">Megjegyzés: Ha egy új DLP-házirendet szeretne implementálni átviteli szabályokkal az EAC-ben, akkor ehelyett használja a [DLP-házirendeket a Biztonsági és megfelelőségi központban](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b2d05-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
