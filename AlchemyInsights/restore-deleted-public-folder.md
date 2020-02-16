---
title: Törölt nyilvános mappa visszaállítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063670"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="75231-102">Törölt nyilvános mappa visszaállítása</span><span class="sxs-lookup"><span data-stu-id="75231-102">Restore a deleted public folder</span></span>

<span data-ttu-id="75231-103">**Törölt elemek visszaállítása nyilvános mappából:**</span><span class="sxs-lookup"><span data-stu-id="75231-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="75231-104">Lásd: Nem lehet visszaállítani a [törölt elemeket egy nem e-mail nyilvános mappából az Outlook 2016-ban.](https://aka.ms/pfrec)</span><span class="sxs-lookup"><span data-stu-id="75231-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="75231-105">**Törölt (bármilyen típusú) nyilvános mappa visszaállítása:**</span><span class="sxs-lookup"><span data-stu-id="75231-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="75231-106">Használja a következő EXO PowerShell parancsot:</span><span class="sxs-lookup"><span data-stu-id="75231-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="75231-107">Szintaxis:</span><span class="sxs-lookup"><span data-stu-id="75231-107">Syntax:</span></span>

    ><span data-ttu-id="75231-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Név -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Elérési út, ahol a mappa vissza lesz állítva></span><span class="sxs-lookup"><span data-stu-id="75231-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="75231-109">Példa: A következő parancs visszaállítja az Almappát1, és a \Parent1 alá helyezi:</span><span class="sxs-lookup"><span data-stu-id="75231-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="75231-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Név -eq "Almappa1"}; Set-PublicFolder $pf.identity -Path \Parent1</span><span class="sxs-lookup"><span data-stu-id="75231-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="75231-111">További részletekért [lásd: Törölt nyilvános mappa visszaállítása.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)</span><span class="sxs-lookup"><span data-stu-id="75231-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
