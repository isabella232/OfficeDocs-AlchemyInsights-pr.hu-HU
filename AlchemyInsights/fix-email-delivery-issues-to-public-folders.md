---
title: E-mail kézbesítési javításokat üzenetet engedélyező nyilvános mappákhoz
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401332"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="98f81-102">E-mail kézbesítési javításokat üzenetet engedélyező nyilvános mappákhoz</span><span class="sxs-lookup"><span data-stu-id="98f81-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="98f81-103">Ha a külső feladóktól nem tudnak üzeneteket küldeni az üzenetet engedélyező nyilvános mappákat, és a feladók hibaüzenet: **nem található (550 5.4.1)**, ellenőrizze az e-mail tartomány számára a nyilvános mappát úgy van beállítva, egy belső továbbítási tartományként helyett egy a tartomány mérvadó:</span><span class="sxs-lookup"><span data-stu-id="98f81-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="98f81-104">Nyissa meg az [Exchange felügyeleti központ (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="98f81-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="98f81-105">Ugrás a **levelezés** \> **elfogadott tartományok**, jelölje ki az elfogadott tartomány, és kattintson a **Szerkesztés**.</span><span class="sxs-lookup"><span data-stu-id="98f81-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="98f81-106">Tulajdonságai lapon, hogy megnyílik, ha **mérvadó**a tartományban típusának beállítása, **belső továbbítási** módosítsa az értéket, és kattintson a **Mentés**.</span><span class="sxs-lookup"><span data-stu-id="98f81-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="98f81-107">Külső feladók **Nincs engedélye (550 5.7.13)** hiba jelenik meg, ha az [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a nyilvános mappában a névtelen felhasználók engedélyeinek megtekintéséhez futtassa a következő parancsot:</span><span class="sxs-lookup"><span data-stu-id="98f81-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="98f81-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Például `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="98f81-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="98f81-109">A külső felhasználók e-mail küldése a nyilvános mappa, adja hozzá a CreateItems hozzáférés jobbra a névtelen felhasználó.</span><span class="sxs-lookup"><span data-stu-id="98f81-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="98f81-110">Használja például a `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` címet.</span><span class="sxs-lookup"><span data-stu-id="98f81-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
