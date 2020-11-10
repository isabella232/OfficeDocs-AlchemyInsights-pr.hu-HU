---
title: A Giphyk használata a Teams-beszélgetésekben
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982507"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="7c25f-102">A Giphyk használata a Teams-beszélgetésekben</span><span class="sxs-lookup"><span data-stu-id="7c25f-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="7c25f-103">Alapértelmezés szerint engedélyezve van a giphyk elérése a Teams-csevegésben.</span><span class="sxs-lookup"><span data-stu-id="7c25f-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="7c25f-104">Rendszergazdaként beállíthatja, hogy a Giphyk a felhasználók számára elérhetők-e az [üzenetküldési házirend megadásával](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) , illetve **a** **giphyk használata a beszélgetésekben funkció használata** esetén.</span><span class="sxs-lookup"><span data-stu-id="7c25f-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="7c25f-105">Ha a Teams-beszélgetések során a GIF-ek nem a várt módon működnek, ellenőrizze az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="7c25f-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="7c25f-106">Az [üzenetküldési házirendnek](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) engedélyeznie kell a giphyk.</span><span class="sxs-lookup"><span data-stu-id="7c25f-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="7c25f-107">A PowerShell-parancsmagok használatával való ellenőrzéshez:</span><span class="sxs-lookup"><span data-stu-id="7c25f-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="7c25f-108">Ellenőrizze, hogy [a PowerShell segítségével kezelheti-e a csoportokat](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="7c25f-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="7c25f-109">Futtassa a PowerShell parancs [Get-CsTeamsMessagingPolicy-identitás globális azonosítóját](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) , és ellenőrizze, hogy a **AllowGiphy** értéke **true**.</span><span class="sxs-lookup"><span data-stu-id="7c25f-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="7c25f-110">Ha a **AllowGiphy** értéke **hamis** , akkor futtassa a következő PowerShell [-CsTeamsMessagingPolicy-identitás globális-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="7c25f-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="7c25f-111">A Giphy URL-címéhez való hozzáférés engedélyezéséhez engedélyezni kell a [választható kapcsolati élményeket](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .</span><span class="sxs-lookup"><span data-stu-id="7c25f-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="7c25f-112">Ha több Teams-üzenetküldési házirendet állított be a bérlői fiókhoz, az érintett felhasználóhoz rendelt házirend identitását határozhatja meg a PowerShell parancs [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Válassza a TeamsMessagingPolicy lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7c25f-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
