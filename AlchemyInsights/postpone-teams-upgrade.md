---
title: Csapatok frissítésének elhalasztása
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
ms.openlocfilehash: fcf724e335bd6a7cb4801d9b2789447befc06ff7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912513"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="9a4ca-102">A Microsoft által vezérelt Teams-frissítés elhalasztása</span><span class="sxs-lookup"><span data-stu-id="9a4ca-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="9a4ca-103">**Fontos:** Segíthetünk a javításhoz egy támogatási diagnosztika használatával, de úgy tűnik, hogy nem használja az Új Felügyeleti központot.</span><span class="sxs-lookup"><span data-stu-id="9a4ca-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="9a4ca-104">Az Új felügyeleti központ használatához csúsztassa a jobb felső sarokban az **új felügyeleti központot** jobbra jelző kapcsolót.</span><span class="sxs-lookup"><span data-stu-id="9a4ca-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="9a4ca-105">Az Új felügyeleti központ segítségével kattintson a **Segítségre van szüksége?** widgetre, írja be a "Csapatok frissítésének elhalasztása" kifejezést, majd kövesse a diagnosztikai eszközök utasításait.</span><span class="sxs-lookup"><span data-stu-id="9a4ca-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="9a4ca-106">Ha a Microsoft által vezérelt automatikus frissítéssel kapcsolatban kapott kommunikációt a Skype Vállalati verzióról a Microsoft Teamsprogramra, és az automatikus frissítést egy későbbi időpontra szeretné halasztani, a globális rendszergazda bejelentkezhet a [Teams Felügyeleti portálra,](https://admin.teams.microsoft.com/dashboard) és miután a Microsoft Teams frissítés e-frissítése gombbal **kiválasztotta** a Frissítés állapotát gombot, válassza a **Halasztás gombot.**</span><span class="sxs-lookup"><span data-stu-id="9a4ca-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="9a4ca-107">A bérlő Microsoft Teamsre történő automatikus frissítésének új dátumának megtekintéséhez frissítse a Teams felügyeleti portállapját.</span><span class="sxs-lookup"><span data-stu-id="9a4ca-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="9a4ca-108">**Megjegyzés:** A **Halasztás** gomb csak akkor érhető el, ha megkapta az üzenetközpont értesítését az automatikus frissítésről.</span><span class="sxs-lookup"><span data-stu-id="9a4ca-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="9a4ca-109">A globális rendszergazdák a [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) programot is futtathatják, hogy többet megtudjanak az aktuális frissítési állapotukról.</span><span class="sxs-lookup"><span data-stu-id="9a4ca-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
