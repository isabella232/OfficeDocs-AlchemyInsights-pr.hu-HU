---
title: Nem lehet hozzáférni a nyilvános mappákhoz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891751"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="28194-102">Az Outlook nem tud nyilvános mappákhoz csatlakozni</span><span class="sxs-lookup"><span data-stu-id="28194-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="28194-103">Ha a nyilvános mappák hoz való hozzáférés egyes felhasználók nál nem működik, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="28194-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="28194-104">Csatlakozzon az EXO PowerShell alkalmazáshoz, és konfigurálja úgy a problémás felhasználói fiók DefaultPublicFolderMailbox paraméterét, hogy az megfeleljen egy működő felhasználói fiók paraméterének.</span><span class="sxs-lookup"><span data-stu-id="28194-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="28194-105">Példa:</span><span class="sxs-lookup"><span data-stu-id="28194-105">Example:</span></span>

<span data-ttu-id="28194-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="28194-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="28194-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<érték az előző parancsból></span><span class="sxs-lookup"><span data-stu-id="28194-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="28194-108">Várjon legalább egy órát, amíg a módosítás érvénybe lép.</span><span class="sxs-lookup"><span data-stu-id="28194-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="28194-109">Ha a probléma továbbra is fennáll, kövesse [az alábbi eljárást](https://aka.ms/pfcte) a nyilvános mappákhoz való hozzáféréssel kapcsolatos problémák megoldásához az Outlook programban.</span><span class="sxs-lookup"><span data-stu-id="28194-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>