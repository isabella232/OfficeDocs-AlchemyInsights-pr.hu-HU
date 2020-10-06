---
title: E-mail-kézbesítési hibák elhárítása levelezési alapú nyilvános mappákban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366466"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="71c31-102">E-mail-kézbesítési hibák elhárítása levelezési alapú nyilvános mappákban</span><span class="sxs-lookup"><span data-stu-id="71c31-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="71c31-103">Ha a külső feladók nem tudnak üzeneteket küldeni a levelezési nyilvános mappákba, és a feladók a következő hibaüzenetet kapják: **nem található (550 5.4.1)**, ellenőrizze, hogy a nyilvános mappa e-mail-tartománya belső továbbító tartományként van-e konfigurálva a mérvadó tartomány helyett:</span><span class="sxs-lookup"><span data-stu-id="71c31-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="71c31-104">Nyissa meg az [Exchange felügyeleti központot (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="71c31-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="71c31-105">Nyissa meg az **e-mail-forgalom** által \> **elfogadott tartományokat**, jelölje ki az elfogadott tartományt, majd kattintson a **Szerkesztés**gombra.</span><span class="sxs-lookup"><span data-stu-id="71c31-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="71c31-106">A megnyíló tulajdonságok lapon, ha a tartomány **mérvadó**értékre van állítva, módosítsa az értéket **belső továbbítóra** , majd kattintson a **Mentés**gombra.</span><span class="sxs-lookup"><span data-stu-id="71c31-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="71c31-107">Ha a külső feladók **nem rendelkeznek engedéllyel (550 5.7.13 hibakódú)**, futtassa az alábbi parancsot az [Exchange Online PowerShellben](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a nyilvános mappában a névtelen felhasználók engedélyeinek megtekintéséhez:</span><span class="sxs-lookup"><span data-stu-id="71c31-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="71c31-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Például: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="71c31-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="71c31-109">Ha engedélyezni szeretné a külső felhasználóknak, hogy e-mailt küldjenek erre a nyilvános mappába, adja meg a CreateItems hozzáférés jogát a felhasználó névtelen számára.</span><span class="sxs-lookup"><span data-stu-id="71c31-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="71c31-110">Használja például a `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` címet.</span><span class="sxs-lookup"><span data-stu-id="71c31-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
