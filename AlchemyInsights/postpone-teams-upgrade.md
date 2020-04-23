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
ms.openlocfilehash: 37263aefe56b673429eb773719413688b72457e7
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785341"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="42596-102">A Microsoft által vezérelt Teams-frissítés elhalasztása</span><span class="sxs-lookup"><span data-stu-id="42596-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="42596-103">Ha a Microsoft által vezérelt automatikus frissítéssel kapcsolatban kapott kommunikációt a Skype Vállalati verzióról a Microsoft Teamsprogramra, és az automatikus frissítést egy későbbi időpontra szeretné halasztani, a globális rendszergazda bejelentkezhet a [Teams Felügyeleti portálra,](https://admin.teams.microsoft.com/dashboard) és miután a Microsoft Teams frissítés e-frissítése gombbal **kiválasztotta** a Frissítés állapotát gombot, válassza a **Halasztás gombot.**</span><span class="sxs-lookup"><span data-stu-id="42596-103">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="42596-104">A bérlő Microsoft Teamsre történő automatikus frissítésének új dátumának megtekintéséhez frissítse a Teams felügyeleti portállapját.</span><span class="sxs-lookup"><span data-stu-id="42596-104">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="42596-105">**Megjegyzés:** A **Halasztás** gomb csak akkor érhető el, ha megkapta az üzenetközpont értesítését az automatikus frissítésről.</span><span class="sxs-lookup"><span data-stu-id="42596-105">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="42596-106">A globális rendszergazdák a [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) programot is futtathatják, hogy többet megtudjanak az aktuális frissítési állapotukról.</span><span class="sxs-lookup"><span data-stu-id="42596-106">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
