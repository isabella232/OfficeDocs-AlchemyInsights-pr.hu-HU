---
title: Csoport létrehozása
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816358"
---
# <a name="create-a-group"></a><span data-ttu-id="97e59-102">Csoport létrehozása</span><span class="sxs-lookup"><span data-stu-id="97e59-102">Create a group</span></span>

<span data-ttu-id="97e59-103">Ez a témakör a csoportok létrehozását ismerteti.</span><span class="sxs-lookup"><span data-stu-id="97e59-103">This topic describes group creation.</span></span>

<span data-ttu-id="97e59-104">**Csoport létrehozására vonatkozó engedély**</span><span class="sxs-lookup"><span data-stu-id="97e59-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="97e59-105">Győződjön meg arról, hogy jogosult új csoport létrehozására.</span><span class="sxs-lookup"><span data-stu-id="97e59-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="97e59-106">A globális rendszergazdák letilthatják a csoportok létrehozását az Azure Portal webhelyen vagy az Access panelen.</span><span class="sxs-lookup"><span data-stu-id="97e59-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="97e59-107">Szükség lehet egy rendszergazdára az új csoport létrehozásához vagy a megfelelő engedélyek létrehozására.</span><span class="sxs-lookup"><span data-stu-id="97e59-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="97e59-108">**Csoport létrehozási engedélyeinek kezelése**</span><span class="sxs-lookup"><span data-stu-id="97e59-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="97e59-109">A globális rendszergazdák kezelhetik a csoportok létrehozásának engedélyét (biztonsági okokból) vagy az Azure Portal vagy a Hozzáférési panelen létrehozott Office 365-csoportokat "A felhasználók biztonsági csoportokat hozhatnak létre az Azure Portálon" vagy a "Felhasználók létrehozhatnak Office 365-csoportokat az Azure Portals webhelyen" lehetőséget választva a Minden csoport általános  >  **(Beállítások)** csoportjában.</span><span class="sxs-lookup"><span data-stu-id="97e59-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="97e59-110">Ha Azure Active Directory P1 Premium-licenccel rendelkezik, korlátozhatja a csoportok létrehozását úgy is, hogy csak egy felhasználócsoportot jelöljön ki.</span><span class="sxs-lookup"><span data-stu-id="97e59-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="97e59-111">**Az office 365-csoport új tagjainak üdvözlő értesítésének letiltása**</span><span class="sxs-lookup"><span data-stu-id="97e59-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="97e59-112">Az Office 365-csoportokba felvett felhasználóknak küldött üdvözlő értesítés letiltható, ha a Powershellben az **UnifiedGroupWelcomeMessageEnabled** beállítást False (Hamis) beállítással tiltja le.</span><span class="sxs-lookup"><span data-stu-id="97e59-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="97e59-113">Erről a beállításról itt [olvashat.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="97e59-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

