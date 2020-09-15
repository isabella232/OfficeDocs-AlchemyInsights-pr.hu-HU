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
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677930"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="bbae9-102">E-mail-kézbesítési hibák elhárítása levelezési alapú nyilvános mappákban</span><span class="sxs-lookup"><span data-stu-id="bbae9-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="bbae9-103">Ha a külső feladók nem tudnak üzeneteket küldeni a levelezési nyilvános mappákba, és a feladók a következő hibaüzenetet kapják: **nem található (550 5.4.1)**, ellenőrizze, hogy a nyilvános mappa e-mail-tartománya belső továbbító tartományként van-e konfigurálva a mérvadó tartomány helyett:</span><span class="sxs-lookup"><span data-stu-id="bbae9-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="bbae9-104">Nyissa meg az [Exchange felügyeleti központot (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="bbae9-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="bbae9-105">Nyissa meg az **e-mail-forgalom** által \> **elfogadott tartományokat**, jelölje ki az elfogadott tartományt, majd kattintson a **Szerkesztés**gombra.</span><span class="sxs-lookup"><span data-stu-id="bbae9-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="bbae9-106">A megnyíló tulajdonságok lapon, ha a tartomány **mérvadó**értékre van állítva, módosítsa az értéket **belső továbbítóra** , majd kattintson a **Mentés**gombra.</span><span class="sxs-lookup"><span data-stu-id="bbae9-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="bbae9-107">Ha a külső feladók **nem rendelkeznek engedéllyel (550 5.7.13 hibakódú)**, futtassa az alábbi parancsot az [Exchange Online PowerShellben](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a nyilvános mappában a névtelen felhasználók engedélyeinek megtekintéséhez:</span><span class="sxs-lookup"><span data-stu-id="bbae9-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="bbae9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Például: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="bbae9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="bbae9-109">Ha engedélyezni szeretné a külső felhasználóknak, hogy e-mailt küldjenek erre a nyilvános mappába, adja meg a CreateItems hozzáférés jogát a felhasználó névtelen számára.</span><span class="sxs-lookup"><span data-stu-id="bbae9-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="bbae9-110">Használja például a `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` címet.</span><span class="sxs-lookup"><span data-stu-id="bbae9-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
