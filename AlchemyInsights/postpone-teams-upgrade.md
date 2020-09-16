---
title: A Teams frissítésének elhalasztása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741773"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="49064-102">A Microsoft-alapú Teams frissítésének elhalasztása</span><span class="sxs-lookup"><span data-stu-id="49064-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="49064-103">**Fontos**: ezt a segítséget akkor tudjuk kijavítani, ha támogatási diagnosztikai lehetőségeket használ, de nem az új felügyeleti központot használja.</span><span class="sxs-lookup"><span data-stu-id="49064-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="49064-104">Ha az új felügyeleti központot szeretné használni, húzza a jobb felső sarokban lévő kapcsolót az **új felügyeleti központ** jobb oldalán.</span><span class="sxs-lookup"><span data-stu-id="49064-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="49064-105">Használja az új felügyeleti központot, és kattintson a **segítségre van szüksége?** elemre, írja be a "elhalasztja a Teams upgrade" parancsot, majd kövesse a megjelenő utasításokat a diagnosztika futtatásához.</span><span class="sxs-lookup"><span data-stu-id="49064-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="49064-106">Ha a Skype vállalati verzióról a Microsoft Teams-re szeretne kommunikálni a Microsoft-alapú automatizált frissítésről, és az automatikus frissítést későbbi dátumra szeretné halasztani, a globális rendszergazda bejelentkezhet a [Teams felügyeleti portálra](https://admin.teams.microsoft.com/dashboard) , és a Microsoft Teams upgrade csoportban a frissítés **állapota** gomb választása után válassza a **Elhalasztva** gombot.</span><span class="sxs-lookup"><span data-stu-id="49064-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="49064-107">Ha szeretné megtekinteni a bérlő automatikus frissítésének új dátumát a Microsoft Teams szolgáltatásban, frissítse a Teams felügyeleti portál lapját.</span><span class="sxs-lookup"><span data-stu-id="49064-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="49064-108">**Megjegyzés:** Az **elhalasztás** gomb csak akkor érhető el, ha az automatikus frissítésről értesítést kapott az üzenetközpont értesítésben.</span><span class="sxs-lookup"><span data-stu-id="49064-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="49064-109">A globális rendszergazdák a [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) is megtekinthetik a jelenlegi frissítés állapotát.</span><span class="sxs-lookup"><span data-stu-id="49064-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
