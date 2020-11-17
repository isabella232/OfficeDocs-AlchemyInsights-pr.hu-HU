---
title: Csoport létrehozása
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088905"
---
# <a name="create-a-group"></a><span data-ttu-id="83dcc-102">Csoport létrehozása</span><span class="sxs-lookup"><span data-stu-id="83dcc-102">Create a group</span></span>

<span data-ttu-id="83dcc-103">Ez a témakör ismerteti a csoportok létrehozását.</span><span class="sxs-lookup"><span data-stu-id="83dcc-103">This topic describes group creation.</span></span>

<span data-ttu-id="83dcc-104">**Csoport létrehozásának engedélye**</span><span class="sxs-lookup"><span data-stu-id="83dcc-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="83dcc-105">Ellenőrizze, hogy jogosult-e új csoport létrehozására.</span><span class="sxs-lookup"><span data-stu-id="83dcc-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="83dcc-106">A globális rendszergazda letilthatja a csoportok létrehozását az Azure portálon vagy az Access-panelen.</span><span class="sxs-lookup"><span data-stu-id="83dcc-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="83dcc-107">Előfordulhat, hogy a rendszergazdának létre kell hoznia az új csoportot, vagy megfelelő engedélyeket kell adnia.</span><span class="sxs-lookup"><span data-stu-id="83dcc-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="83dcc-108">**Csoport létrehozási engedélyeinek kezelése**</span><span class="sxs-lookup"><span data-stu-id="83dcc-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="83dcc-109">A globális rendszergazdák kezelhetik a csoport létrehozásához szükséges engedélyeket (biztonsági okokból kifolyólag) vagy az Azure portálon vagy az Access-munkaablakban létrehozott Office 365-csoportokat, ha a "felhasználók létrehozhatnak biztonsági csoportokat az Azure-portálokon" vagy a "felhasználók létrehozhatnak Office 365-csoportokat az Azure portálokon" az **összes csoport**  >  **általános (beállítások)** parancsára kattintva.</span><span class="sxs-lookup"><span data-stu-id="83dcc-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="83dcc-110">A csoportok létrehozását úgy is korlátozhatja, hogy a felhasználók egy csoportját kijelölje, ha az Azure Active Directory P1 prémium licenccel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="83dcc-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="83dcc-111">**Az új Office 365-csoporttagok üdvözlő értesítésének letiltása**</span><span class="sxs-lookup"><span data-stu-id="83dcc-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="83dcc-112">Az Office 365-csoportokba felvett felhasználóknak küldött üdvözlő értesítést a PowerShell **UnifiedGroupWelcomeMessageEnabled** false értékre állításával lehet letiltani.</span><span class="sxs-lookup"><span data-stu-id="83dcc-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="83dcc-113">[Ebben a beállításban](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)tájékozódhat.</span><span class="sxs-lookup"><span data-stu-id="83dcc-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

