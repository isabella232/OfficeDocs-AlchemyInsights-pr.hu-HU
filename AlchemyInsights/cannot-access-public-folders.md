---
title: A nyilvános mappák nem férhető hozzá
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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959497"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="00be1-102">Az Outlook nem tud kapcsolódni a nyilvános mappákhoz.</span><span class="sxs-lookup"><span data-stu-id="00be1-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="00be1-103">Ha a nyilvános mappához való hozzáférés néhány felhasználó esetében nem működik, próbálkozzon a következőkkel:</span><span class="sxs-lookup"><span data-stu-id="00be1-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="00be1-104">Csatlakozzon az EXO PowerShell környezethez, és konfigurálja a DefaultPublicFolderMailbox eszközt a problémás felhasználói fiókban úgy, hogy az megfeleljen egy működő felhasználói fióknak.</span><span class="sxs-lookup"><span data-stu-id="00be1-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="00be1-105">Példa:</span><span class="sxs-lookup"><span data-stu-id="00be1-105">Example:</span></span>

<span data-ttu-id="00be1-106">Kap-postaláda WorkingUser | Ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="00be1-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="00be1-107">Állítsa be a postafiók ProblemUser-DefaultPublicFolderMailbox \<értékét az előző parancsból></span><span class="sxs-lookup"><span data-stu-id="00be1-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="00be1-108">Várjon legalább egy órát a változtatás érvénybe léptetéséhez.</span><span class="sxs-lookup"><span data-stu-id="00be1-108">Wait at least one hour for the change to take effect.</span></span>