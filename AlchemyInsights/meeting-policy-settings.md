---
title: Értekezletházirend-beállításai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042846"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="672a2-102">Értekezlet-szabályzatok kezelése a Microsoft Teamsben</span><span class="sxs-lookup"><span data-stu-id="672a2-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="672a2-103">**Megjegyzés: Akár 24 órát is igénybe vehet, amíg a házirend-módosítások érvénybe lépnek a felhasználók számára.**</span><span class="sxs-lookup"><span data-stu-id="672a2-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="672a2-104">Előfordulhat, hogy nem tudja azonnal módosítani az újonnan létrehozott házirendeket; várjon 4 órát, és próbálja meg újra módosítani az újonnan létrehozott házirendet.</span><span class="sxs-lookup"><span data-stu-id="672a2-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="672a2-105">Az értekezlet-házirendek a szervezet felhasználói által ütemezett értekezletek résztvevői számára elérhető funkciók szabályozására szolgálnak.</span><span class="sxs-lookup"><span data-stu-id="672a2-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="672a2-106">Előfordulhat, hogy az értekezlet-házirendek egyes funkciói még nincsenek megvalósítva a Teams felügyeleti központban (ezek a dokumentációban a "hamarosan" címkével vannak ellátva).</span><span class="sxs-lookup"><span data-stu-id="672a2-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="672a2-107">Ebben az esetben, vagy ha olyan hibaüzenetjelenik meg, mint a "Jelenleg nem tudjuk frissíteni a szabályzatot, de próbálkozzon később" a Microsoft Teams felügyeleti központban, azt javasoljuk, hogy a PowerShell használatával hozzon létre vagy módosítsa a Teams értekezlet-szabályzatait.</span><span class="sxs-lookup"><span data-stu-id="672a2-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="672a2-108">Az értekezlet-szabályzatokról az alábbi forrásokban talál további információt:</span><span class="sxs-lookup"><span data-stu-id="672a2-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="672a2-109">Ha többet szeretne tudni a házirendek létrehozásáról, a módosításokról és a felhasználók házirendhez való hozzárendeléséről, olvassa el [Az értekezlet-irányelvek kezelése a Csoportokban című témakört.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="672a2-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="672a2-110">Ha a PowerShell-parancsmagokkal szeretne házirend-módosításokat végrehajtani, olvassa el a [Teams PowerShell – áttekintés című témakört.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="672a2-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="672a2-111">A [Skype Vállalati verzió PowerShell-modult](https://www.microsoft.com/download/details.aspx?id=39366) kell használnia a Teams értekezlet-szabályzataihoz.</span><span class="sxs-lookup"><span data-stu-id="672a2-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="672a2-112">További információt a [\*-CsTeamsMeetingPolicy parancsmagok dokumentációjában](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) talál.</span><span class="sxs-lookup"><span data-stu-id="672a2-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

