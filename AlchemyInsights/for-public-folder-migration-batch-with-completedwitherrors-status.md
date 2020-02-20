---
title: Befejezett hiba állapotú nyilvános mappa áttelepítési köteg esetén
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
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158610"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="8af72-102">Befejezett hiba állapotú nyilvános mappa áttelepítési köteg esetén</span><span class="sxs-lookup"><span data-stu-id="8af72-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="8af72-103">A köteg befejezéséhez kövesse az alábbi lépéseket, kihagyva a nagy/rossz elemeket:</span><span class="sxs-lookup"><span data-stu-id="8af72-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="8af72-104">Az áttelepítési köteg kihagyott elemeinek jóváhagyása:</span><span class="sxs-lookup"><span data-stu-id="8af72-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="8af72-105">A következő paranccsal hagyhatja jóvá a "Szinkronizált" de nem befejezett áttelepítési kérelmek kihagyott elemeit:</span><span class="sxs-lookup"><span data-stu-id="8af72-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="8af72-106">Az áttelepítési köteg nek és a kérelmeknek néhány perc alatt újra kell kezdődnie és befejeződniük.</span><span class="sxs-lookup"><span data-stu-id="8af72-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

