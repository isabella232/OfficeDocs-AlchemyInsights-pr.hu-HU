---
title: 'Csapatok frissítésének elhalasztása '
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: 27f3dc123590f3199d6a984d7e9a4db3918ac9cb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758864"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="ef85d-102">A Microsoft által vezérelt Teams-frissítés elhalasztása</span><span class="sxs-lookup"><span data-stu-id="ef85d-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="ef85d-103">Ha a Microsoft által vezérelt automatikus frissítésről kapott kommunikációt a Skype Vállalati verzióról a Microsoft Teamsre, és az automatikus frissítést egy későbbi időpontra szeretné halasztani, globális rendszergazdája bejelentkezhet a [Teams Felügyeleti portálra,](https://admin.teams.microsoft.com/dashboard) és kiválaszthatja a **Halasztás gombot.**</span><span class="sxs-lookup"><span data-stu-id="ef85d-103">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and select the **Postpone** button.</span></span> <span data-ttu-id="ef85d-104">A bérlő Microsoft Teamsre történő automatikus frissítésének új dátumának megtekintéséhez frissítse a Teams felügyeleti portállapját.</span><span class="sxs-lookup"><span data-stu-id="ef85d-104">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="ef85d-105">**Megjegyzés:** A **Halasztás** gomb csak akkor érhető el, ha megkapta az üzenetközpont értesítését az automatikus frissítésről.</span><span class="sxs-lookup"><span data-stu-id="ef85d-105">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="ef85d-106">A globális rendszergazdák a [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) programot is futtathatják, hogy többet megtudjanak az aktuális frissítési állapotukról.</span><span class="sxs-lookup"><span data-stu-id="ef85d-106">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span> 