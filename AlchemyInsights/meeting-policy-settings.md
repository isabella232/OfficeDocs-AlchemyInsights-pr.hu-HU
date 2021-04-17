---
title: Értekezleti házirend beállításai
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825445"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="e4f37-102">Értekezleti házirendek kezelése a Microsoft Teamsben</span><span class="sxs-lookup"><span data-stu-id="e4f37-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="e4f37-103">**Megjegyzés: Akár 24 óra is elehet, hogy a házirendek módosításai életbe lépnek a felhasználóknál.**</span><span class="sxs-lookup"><span data-stu-id="e4f37-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="e4f37-104">Előfordulhat, hogy az újonnan létrehozott házirendeket nem tudja azonnal módosításokat létrehozni; Várjon 4 órát, és próbálja meg ismét módosítani az újonnan létrehozott házirendet.</span><span class="sxs-lookup"><span data-stu-id="e4f37-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="e4f37-105">Az értekezleti házirendek a szervezet felhasználói által ütemezett értekezletek résztvevői számára elérhető funkciók szabályozását szolgálják.</span><span class="sxs-lookup"><span data-stu-id="e4f37-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="e4f37-106">Előfordulhat, hogy az értekezleti házirendek egyes funkcióit még nem hajtják végre a Teams Felügyeleti központban (ezeket a dokumentációban "hamarosan" felirat jelöli).</span><span class="sxs-lookup"><span data-stu-id="e4f37-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="e4f37-107">Ebben az esetben, vagy ha a Microsoft Teams Felügyeleti központban a következőhöz hasonló hibaüzenet jelenik meg: "Jelenleg nem tudjuk frissíteni a házirendet, de később újra megpróbáljuk", azt javasoljuk, hogy a PowerShell használatával hozzon létre vagy módosítson Teams-értekezleti házirendeket.</span><span class="sxs-lookup"><span data-stu-id="e4f37-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="e4f37-108">Az értekezleti házirendekről az alábbi forrásokban talál további információt:</span><span class="sxs-lookup"><span data-stu-id="e4f37-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="e4f37-109">Ha többet szeretne tudni a házirendek létrehozásáról, a módosításokról és a felhasználók házirendhez való hozzárendelésről, olvassa el az Értekezleti házirendek kezelése [a Teamsben részt.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="e4f37-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="e4f37-110">A házirendek PowerShell-parancsmagokkal való módosításairól A Teams PowerShell áttekintése [témakörben olvashat.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="e4f37-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="e4f37-111">A Teams-értekezleti [házirendekhez](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) a Skype Vállalati verzió PowerShell modulját kell használnia.</span><span class="sxs-lookup"><span data-stu-id="e4f37-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="e4f37-112">További információt [a \*-CsTeamsMeetingPolicy parancsmagok](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentációjában talál.</span><span class="sxs-lookup"><span data-stu-id="e4f37-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

