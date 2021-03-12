---
title: Értekezleti házirend beállításai
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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704608"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="b3773-102">Értekezleti házirendek kezelése a Microsoft Teamsben</span><span class="sxs-lookup"><span data-stu-id="b3773-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="b3773-103">**Megjegyzés: Akár 24 óra is elehet, hogy a házirend módosításai életbe lépnek a felhasználóknál.**</span><span class="sxs-lookup"><span data-stu-id="b3773-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="b3773-104">Előfordulhat, hogy nem lehet azonnal módosításokat létrehozni az újonnan létrehozott házirendeket; várjon 4 órát, és próbálja meg ismét módosítani az újonnan létrehozott házirendet.</span><span class="sxs-lookup"><span data-stu-id="b3773-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="b3773-105">Az értekezleti házirendek a szervezet felhasználói által ütemezett értekezletek résztvevői számára elérhető funkciók szabályozását szolgálják.</span><span class="sxs-lookup"><span data-stu-id="b3773-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="b3773-106">Előfordulhat, hogy az értekezleti házirendek egyes funkcióit még nem hajtják végre a Teams Felügyeleti központban (ezeket a dokumentációban "hamarosan" felirattal jelölték).</span><span class="sxs-lookup"><span data-stu-id="b3773-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="b3773-107">Ebben az esetben, vagy ha a Microsoft Teams Felügyeleti központban a következőhöz hasonló hibaüzenet jelenik meg: "Jelenleg nem tudjuk frissíteni a házirendet, de később újra megpróbáljuk", azt javasoljuk, hogy a PowerShell használatával hozzon létre vagy módosítson Teams-értekezleti házirendeket.</span><span class="sxs-lookup"><span data-stu-id="b3773-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="b3773-108">Az értekezleti házirendekkel kapcsolatos további információkért lásd az alábbi forrásokat:</span><span class="sxs-lookup"><span data-stu-id="b3773-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="b3773-109">Ha többet szeretne tudni a házirendek létrehozásáról, a módosításokról és a felhasználók házirendhez való hozzárendelésről, olvassa el az Értekezleti házirendek kezelése [a Teamsben.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="b3773-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="b3773-110">A házirendEk PowerShell-parancsmagokkal való módosításairól a Teams PowerShell áttekintése [nyújt áttekintést.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="b3773-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="b3773-111">A Skype Vállalati [verzió PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) modulját kell használnia a Teams-értekezleti házirendek esetén.</span><span class="sxs-lookup"><span data-stu-id="b3773-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="b3773-112">További információt [a \*-CsTeamsMeetingPolicy parancsmagok dokumentációjában](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) talál.</span><span class="sxs-lookup"><span data-stu-id="b3773-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

