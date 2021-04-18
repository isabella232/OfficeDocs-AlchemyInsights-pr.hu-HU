---
title: A nyilvános mappákhoz való hozzáférés szabályozása az Outlook használatával
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816742"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="2f173-102">A nyilvános mappákhoz való hozzáférés szabályozása az Outlook használatával</span><span class="sxs-lookup"><span data-stu-id="2f173-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="2f173-103">A nyilvános mappákhoz hozzáférő felhasználók szabályozásához az Outlook használatával:</span><span class="sxs-lookup"><span data-stu-id="2f173-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="2f173-104">A `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` használata</span><span class="sxs-lookup"><span data-stu-id="2f173-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="2f173-105">$true: Nyilvános mappák elérésének engedélyezése a felhasználóknak az Outlookban</span><span class="sxs-lookup"><span data-stu-id="2f173-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="2f173-106">$false: A nyilvános mappák elérésének megakadályozása az Outlookban.</span><span class="sxs-lookup"><span data-stu-id="2f173-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="2f173-107">Ez az alapértelmezett érték.</span><span class="sxs-lookup"><span data-stu-id="2f173-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="2f173-108">Megjegyzés: Ez az eljárás csak a Windows rendszerű asztali Outlook kapcsolatokat szabályozhatja.</span><span class="sxs-lookup"><span data-stu-id="2f173-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="2f173-109">A felhasználók továbbra is hozzáférhetnek a nyilvános mappákhoz az OWA vagy a Mac Outlook használatával.</span><span class="sxs-lookup"><span data-stu-id="2f173-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="2f173-110">További információért lásd: [Ellenőrzött kapcsolatok a nyilvános mappákkal az Outlookban](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="2f173-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
