---
title: Értekezlet-házirend beállításai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627576"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="63d56-102">Értekezletházirendek kezelése a Microsoft teamben</span><span class="sxs-lookup"><span data-stu-id="63d56-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="63d56-103">Az értekezletre vonatkozó házirendek a szervezet felhasználói által ütemezett értekezletekhez rendelkezésre álló szolgáltatások vezérlésének ellenőrzésére szolgálnak.</span><span class="sxs-lookup"><span data-stu-id="63d56-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="63d56-104">Az értekezletre vonatkozó házirendek egyes funkciói még nem valósulhatnak meg a csapatok admin központban (ezeket a dokumentációban "hamarosan" felirattal kell címkézni).</span><span class="sxs-lookup"><span data-stu-id="63d56-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="63d56-105">Ebben az esetben, vagy ha Ön szerzés egy hiba szeret "mi vidám ' korszerűsíteni a politika éppen most de megpróbál ez újra később"-ban Mikroszkóp fuvaros admin központ, mi ajánl amit ön használ PowerShell-hoz teremt vagy módosít fuvaros találkozó politikák.</span><span class="sxs-lookup"><span data-stu-id="63d56-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="63d56-106">A következő forrásokból tájékozódhat az értekezletre vonatkozó házirendekkel kapcsolatban:</span><span class="sxs-lookup"><span data-stu-id="63d56-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="63d56-107">A házirendek létrehozásával, a módosításokkal és a felhasználóknak a házirendhez való hozzárendelésével kapcsolatos tudnivalókat [az értekezletházirendek kezelése a csapatokban](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="63d56-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="63d56-108">A házirendek módosításának PowerShell-parancsmagokkal való használatához lásd a [csapatok PowerShell – áttekintés](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)című témakört.</span><span class="sxs-lookup"><span data-stu-id="63d56-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="63d56-109">Meg kell használni a [Skype for Business PowerShell modult](https://www.microsoft.com/download/details.aspx?id=39366) az olyan csapatoknak, amelyek a házirendeket tárgyalnak.</span><span class="sxs-lookup"><span data-stu-id="63d56-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="63d56-110">A további tudnivalókért tanulmányozza a [\*-csteamsmeetingpolicy parancsmagok dokumentációját](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="63d56-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="63d56-111">**Megjegyzés:** A házirend-módosítások érvénybe léptetéséhez akár 24 óráig is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="63d56-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="63d56-112">Előfordulhat, hogy azonnal nem tudja módosítani az újonnan létrehozott házirendeket; várjon 4 órát, majd próbálja meg újra módosítani az újonnan létrehozott házirendet.</span><span class="sxs-lookup"><span data-stu-id="63d56-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="63d56-113">Ha-a ' csendes birtoklás probléma, megpróbál PowerShell.</span><span class="sxs-lookup"><span data-stu-id="63d56-113">If you're still having problems, try PowerShell.</span></span>  