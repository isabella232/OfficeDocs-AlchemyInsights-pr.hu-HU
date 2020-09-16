---
title: Értekezlet-házirend beállításai
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794336"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="5874e-102">Értekezlet-házirendek kezelése a Microsoft Teams alkalmazásban</span><span class="sxs-lookup"><span data-stu-id="5874e-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="5874e-103">**Megjegyzés: akár 24 óra is eltelhet, amíg a házirend módosítása a felhasználók számára érvényben lesz.**</span><span class="sxs-lookup"><span data-stu-id="5874e-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="5874e-104">Előfordulhat, hogy nem tudja azonnal módosítani az újonnan létrehozott házirendeket; várjon 4 órát, és próbálja meg ismét módosítani az újonnan létrehozott házirendet.</span><span class="sxs-lookup"><span data-stu-id="5874e-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="5874e-105">Az értekezlet-házirendek a szervezet felhasználói által ütemezett értekezletekhez a résztvevők számára elérhető funkciók szabályozására szolgálnak.</span><span class="sxs-lookup"><span data-stu-id="5874e-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="5874e-106">Az értekezlet-összehívások bizonyos funkciói nem hajthatók végre a Teams felügyeleti központban, (ezeket a "hamarosan elérhető" felirat jelzi a dokumentációban).</span><span class="sxs-lookup"><span data-stu-id="5874e-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="5874e-107">Ebben az esetben, vagy ha hibaüzenetet kap, például "nem tudjuk frissíteni a házirendet, de később újra próbálkozni", a Microsoft Teams felügyeleti központjában azt javasoljuk, hogy a PowerShell segítségével hozza létre vagy módosítsa a Teams-értekezletekre vonatkozó házirendeket.</span><span class="sxs-lookup"><span data-stu-id="5874e-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="5874e-108">Az értekezlet-házirendekről további információt az alábbi forrásokban talál:</span><span class="sxs-lookup"><span data-stu-id="5874e-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="5874e-109">Ha tudni szeretné, hogy miként hozhat létre házirendeket, és hogyan módosíthatja a felhasználókat a házirendhez, olvassa el az [értekezlet-házirendek kezelése a Teams alkalmazásban](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)című témakört.</span><span class="sxs-lookup"><span data-stu-id="5874e-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="5874e-110">Ha PowerShell-parancsmagokkal szeretné módosítani a házirendet, olvassa el a [Teams PowerShell áttekintése](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)című témakört.</span><span class="sxs-lookup"><span data-stu-id="5874e-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="5874e-111">A Teams Meeting-házirendjeihez a [Skype vállalati verzió PowerShell-modult](https://www.microsoft.com/download/details.aspx?id=39366) kell használnia.</span><span class="sxs-lookup"><span data-stu-id="5874e-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="5874e-112">További információért tekintse át a [\*-CsTeamsMeetingPolicy parancsmagok dokumentációját](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="5874e-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

