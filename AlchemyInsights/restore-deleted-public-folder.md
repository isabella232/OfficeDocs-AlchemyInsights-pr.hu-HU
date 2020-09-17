---
title: Törölt nyilvános mappa visszaállítása
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
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774533"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="56a12-102">Törölt nyilvános mappa visszaállítása</span><span class="sxs-lookup"><span data-stu-id="56a12-102">Restore a deleted public folder</span></span>

<span data-ttu-id="56a12-103">**Törölt elemek visszaállítása nyilvános mappából**:</span><span class="sxs-lookup"><span data-stu-id="56a12-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="56a12-104">Lásd: nem lehet [törölt elemeket visszaállítani egy nem levelezési nyilvános mappából az Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="56a12-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="56a12-105">**Törölt nyilvános mappa (bármilyen típus) visszaállítása**:</span><span class="sxs-lookup"><span data-stu-id="56a12-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="56a12-106">Kérjük, használja az EXO PowerShell következő parancsát:</span><span class="sxs-lookup"><span data-stu-id="56a12-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="56a12-107">Szintaxisa</span><span class="sxs-lookup"><span data-stu-id="56a12-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="56a12-108">Példa: a következő parancs visszaállítja a Subfolder1-ot, és a \Parent1 alá helyezi:</span><span class="sxs-lookup"><span data-stu-id="56a12-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="56a12-109">További információt a [törölt nyilvános mappa visszaállítása](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="56a12-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
