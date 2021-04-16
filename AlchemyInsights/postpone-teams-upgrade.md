---
title: A Teams frissítésének elhalasztása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801233"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="2fdb0-102">A Microsoft-alapú Teams-frissítés elhalasztása</span><span class="sxs-lookup"><span data-stu-id="2fdb0-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="2fdb0-103">**Fontos:** Segíthetünk a hiba kijavításában egy támogatási diagnosztikai eszköz használatával, de úgy tűnik, hogy ön nem az Új felügyeleti központot használja.</span><span class="sxs-lookup"><span data-stu-id="2fdb0-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="2fdb0-104">Az Új felügyeleti központ megnyitásához húzza a jobb felső  sarokban az Új felügyeleti központ csúszkával jobbra található kapcsolót.</span><span class="sxs-lookup"><span data-stu-id="2fdb0-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="2fdb0-105">Az Új felügyeleti központban kattintson a Segítségre van **szüksége?** vezérlőre, írja be a "Teams-frissítés elhalasztása" parancsot, majd az utasításokat használva futtassa a diagnosztikai adatokat.</span><span class="sxs-lookup"><span data-stu-id="2fdb0-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="2fdb0-106">Ha a Microsoft által vezetett automatikus frissítésről kapott kommunikációt a Skype Vállalati verzióról a Microsoft Teamsre, és későbbre szeretné halasztani az  automatikus frissítést, a globális  rendszergazda bejelentkezhet a [Teams](https://admin.teams.microsoft.com/dashboard) felügyeleti portálra, és miután a Microsoft Teams Frissítés csoportban a Frissítési állapot gombra kattintott, válassza a Elhalasztás gombot.</span><span class="sxs-lookup"><span data-stu-id="2fdb0-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="2fdb0-107">A Teams felügyeleti portál lapját frissítve láthatja a bérlői fiók Microsoft Teamsre való automatikus frissítésének új dátumát.</span><span class="sxs-lookup"><span data-stu-id="2fdb0-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="2fdb0-108">**Megjegyzés:** A **Halasztás** gomb csak akkor érhető el, ha megkapta az üzenetközpont értesítését az automatikus frissítésről.</span><span class="sxs-lookup"><span data-stu-id="2fdb0-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="2fdb0-109">A globális rendszergazdák a [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) futtatásával is tudnak többet megtudni aktuális frissítési állapotukról.</span><span class="sxs-lookup"><span data-stu-id="2fdb0-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
