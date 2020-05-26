---
title: Üdvözlőüzenet a Microsoft 365-csoportokban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357843"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="d3189-102">Üdvözlőüzenet a Microsoft 365-csoportokban</span><span class="sxs-lookup"><span data-stu-id="d3189-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="d3189-103">A Microsoft 365 csoporthoz csatlakozó új felhasználók üdvözlő e-mailt kapnak, ha a "UnifiedGroupWelcomeMessageEnabled" tulajdonság igaz.</span><span class="sxs-lookup"><span data-stu-id="d3189-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="d3189-104">Ha le szeretné tiltani az üdvözlőüzenetet, használja a következő [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) parancsot:</span><span class="sxs-lookup"><span data-stu-id="d3189-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
