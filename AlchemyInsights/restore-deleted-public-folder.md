---
title: Törölt nyilvános mappa visszaállítása
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
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809441"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="4ff83-102">Törölt nyilvános mappa visszaállítása</span><span class="sxs-lookup"><span data-stu-id="4ff83-102">Restore a deleted public folder</span></span>

<span data-ttu-id="4ff83-103">**Törölt elemek visszaállítása nyilvános mappából:**</span><span class="sxs-lookup"><span data-stu-id="4ff83-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="4ff83-104">Lásd: [Az Outlook 2016-ban](https://aka.ms/pfrec)nem lehet helyreállítani a nem levelezési nyilvános mappából törölt elemeket.</span><span class="sxs-lookup"><span data-stu-id="4ff83-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="4ff83-105">**Törölt nyilvános mappa (bármilyen típusú)** visszaállítása:</span><span class="sxs-lookup"><span data-stu-id="4ff83-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="4ff83-106">Használja a következő EXO PowerShell-parancsot:</span><span class="sxs-lookup"><span data-stu-id="4ff83-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="4ff83-107">Szintaxis:</span><span class="sxs-lookup"><span data-stu-id="4ff83-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="4ff83-108">Példa: A következő paranccsal visszaállíthatja az Almappa1 mappáját, és a \Parent1 mappába adhatja:</span><span class="sxs-lookup"><span data-stu-id="4ff83-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="4ff83-109">További [részletekért lásd:](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) Törölt nyilvános mappa visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="4ff83-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
