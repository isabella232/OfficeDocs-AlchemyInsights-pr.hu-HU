---
title: Nyilvános mappa engedélyeinek módosítása
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714249"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="8828d-102">Nyilvános mappa engedélyeinek módosítása</span><span class="sxs-lookup"><span data-stu-id="8828d-102">Changing public folder permissions</span></span>

<span data-ttu-id="8828d-103">A nyilvános mappák engedélyei a felhasználók és a rendszergazdák által módosíthatók az Outlookban.</span><span class="sxs-lookup"><span data-stu-id="8828d-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="8828d-104">A rendszergazdák az alábbi módon is szabályozhatják az engedélyeket az Exchange felügyeleti központból (EAC):</span><span class="sxs-lookup"><span data-stu-id="8828d-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="8828d-105">A Microsoft 365 felügyeleti központban nyissa meg a **felügyeleti központok** \> **Exchange**-et.</span><span class="sxs-lookup"><span data-stu-id="8828d-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="8828d-106">Válassza a **nyilvános mappák**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8828d-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="8828d-107">Itt módosíthatja az egyes nyilvános mappák engedélyeit úgy, hogy a biztonsági csoportokat hozzárendeli az engedélyekhez.</span><span class="sxs-lookup"><span data-stu-id="8828d-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="8828d-108">Ahhoz, hogy egy végfelhasználó módosítsa a nyilvános mappa engedélyeit, a felhasználónak rendelkeznie kell a mappára vonatkozó tulajdonosi jogosultságokkal.</span><span class="sxs-lookup"><span data-stu-id="8828d-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="8828d-109">A nyilvános mappa engedélyeinek elhárítása című témakörben ismertetett lépéseket követve [diagnosztizálhatja és elháríthatja a nyilvános mappákkal kapcsolatos engedélyeket](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) .</span><span class="sxs-lookup"><span data-stu-id="8828d-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="8828d-110">**Megjegyzés**: számos ismert probléma merülhet fel a nyilvános mappák engedélyeinek módosításakor.</span><span class="sxs-lookup"><span data-stu-id="8828d-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="8828d-111">További információt az alábbi cikkekben találhat.</span><span class="sxs-lookup"><span data-stu-id="8828d-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="8828d-112">Nem lehet engedélyeket alkalmazni a nyilvános mappák almappáira az EAC-ban</span><span class="sxs-lookup"><span data-stu-id="8828d-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="8828d-113">"A postaláda nem található meg a helyi erdőben" hibaüzenet jelenik meg a nyilvános mappák elérése során</span><span class="sxs-lookup"><span data-stu-id="8828d-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
