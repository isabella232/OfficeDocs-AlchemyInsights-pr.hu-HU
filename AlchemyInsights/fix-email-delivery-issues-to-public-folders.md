---
title: E-mail kézbesítési javításokat üzenetet engedélyező nyilvános mappákhoz
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525110"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="b61e0-102">E-mail kézbesítési javításokat üzenetet engedélyező nyilvános mappákhoz</span><span class="sxs-lookup"><span data-stu-id="b61e0-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="b61e0-103">Ha a külső feladóktól nem tudnak üzeneteket küldeni az üzenetet engedélyező nyilvános mappákat, és a feladók hibaüzenet: **nem található (550 5.4.1)**, ellenőrizze az e-mail tartomány számára a nyilvános mappát úgy van beállítva, egy belső továbbítási tartományként helyett egy a tartomány mérvadó:</span><span class="sxs-lookup"><span data-stu-id="b61e0-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="b61e0-104">Nyissa meg az [Exchange felügyeleti központ (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="b61e0-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="b61e0-105">Ugrás a **levelezés** \> **elfogadott tartományok**, jelölje ki az elfogadott tartomány, és kattintson a **Szerkesztés**.</span><span class="sxs-lookup"><span data-stu-id="b61e0-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="b61e0-106">Tulajdonságai lapon, hogy megnyílik, ha **mérvadó**a tartományban típusának beállítása, **belső továbbítási** módosítsa az értéket, és kattintson a **Mentés**.</span><span class="sxs-lookup"><span data-stu-id="b61e0-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="b61e0-107">Külső feladók **Nincs engedélye (550 5.7.13)** hiba jelenik meg, ha az [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a nyilvános mappában a névtelen felhasználók engedélyeinek megtekintéséhez futtassa a következő parancsot:</span><span class="sxs-lookup"><span data-stu-id="b61e0-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="b61e0-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Például `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="b61e0-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="b61e0-109">A külső felhasználók e-mail küldése a nyilvános mappa, adja hozzá a CreateItems hozzáférés jobbra a névtelen felhasználó.</span><span class="sxs-lookup"><span data-stu-id="b61e0-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="b61e0-110">Használja például a `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` címet.</span><span class="sxs-lookup"><span data-stu-id="b61e0-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
