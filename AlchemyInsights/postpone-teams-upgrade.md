---
title: 'Csapatfrissítések elhalasztása '
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
ms.openlocfilehash: 28c3a376170aba0ae43929865200fc85cd1c41f4
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626746"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="0c009-102">A Microsoft által vezérelt csapatok frissítésének elhalasztása</span><span class="sxs-lookup"><span data-stu-id="0c009-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="0c009-103">Ha a Skype for Business és a Microsoft csapatok között a Microsoft által vezérelt automatikus frissítéssel kapcsolatban kapott tájékoztatást, és szeretné elhalasztani az automatikus frissítést egy későbbi időpontra, az Office 365 globális rendszergazda bejelentkezhet a [csapatok admin portálra](https://admin.teams.microsoft.com/dashboard) , és kiválaszthatja a **Elhalasztva** gombot.</span><span class="sxs-lookup"><span data-stu-id="0c009-103">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Office 365 Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and select the **Postpone** button.</span></span> <span data-ttu-id="0c009-104">Ha meg szeretné tudni, hogy a bérlő automatikus frissítése a Microsoft csapatai számára milyen új dátumot kíván, frissítse a csapatok rendszergazdai portáloldalát.</span><span class="sxs-lookup"><span data-stu-id="0c009-104">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="0c009-105">**Megjegyzés:** Az **elhalasztás** gomb csak akkor lesz elérhető, ha megkapta az üzenetközpont értesítését az automatikus frissítéssel kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="0c009-105">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="0c009-106">Office 365 globális adminok is futtatható [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) , hogy többet tudjon meg a jelenlegi frissítési állapot.</span><span class="sxs-lookup"><span data-stu-id="0c009-106">Office 365 Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span> 