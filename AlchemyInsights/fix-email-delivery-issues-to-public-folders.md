---
title: A levelezésre képes nyilvános mappákba történő kézbesítési problémák megoldása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716354"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="c1078-102">A levelezésre képes nyilvános mappákba történő kézbesítési problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="c1078-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="c1078-103">Ha a külső feladók nem tudnak üzeneteket küldeni a levelezést támogató nyilvános mappákba, és a feladóak a következő hibaüzenetet kapják: **nem található (550 5.4.1),** ellenőrizze, hogy a nyilvános mappa e-mail tartománya belső továbbítótartományként van-e-e konfigurálva a mérvadó tartomány helyett:</span><span class="sxs-lookup"><span data-stu-id="c1078-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="c1078-104">Nyissa meg az [Exchange Felügyeleti központot (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)</span><span class="sxs-lookup"><span data-stu-id="c1078-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="c1078-105">Nyissa meg a **Levelezési folyamat** \> Elfogadott tartományok at, jelölje ki az elfogadott **tartományt,** majd kattintson a **Szerkesztés gombra.**</span><span class="sxs-lookup"><span data-stu-id="c1078-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="c1078-106">Ha a megnyíló tulajdonságlapon a tartománytípus **Mérvadó**értékre van állítva, módosítsa az értéket **Belső továbbításra,** majd kattintson a **Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="c1078-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="c1078-107">Ha a külső feladók megkapják azt a **hibát, amelyhez nincs engedélye (550 5.7.13),** futtassa a következő parancsot az [Exchange Online PowerShellben](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a névtelen felhasználók engedélyeimegtekintéséhez a nyilvános mappában:</span><span class="sxs-lookup"><span data-stu-id="c1078-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="c1078-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous``Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`Például.</span><span class="sxs-lookup"><span data-stu-id="c1078-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="c1078-109">Ha azt szeretné, hogy a külső felhasználók e-mailt küldhessenek ebbe a nyilvános mappába, adja hozzá a CreateItems hozzáférési jogot a Névtelen felhasználóhoz.</span><span class="sxs-lookup"><span data-stu-id="c1078-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="c1078-110">Használja például a `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` címet.</span><span class="sxs-lookup"><span data-stu-id="c1078-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
