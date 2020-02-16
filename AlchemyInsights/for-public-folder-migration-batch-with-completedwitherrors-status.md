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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043593"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="560d5-102">Befejezett hiba állapotú nyilvános mappa áttelepítési köteg esetén</span><span class="sxs-lookup"><span data-stu-id="560d5-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="560d5-103">A köteg befejezéséhez kövesse az alábbi lépéseket, kihagyva a nagy/rossz elemeket:</span><span class="sxs-lookup"><span data-stu-id="560d5-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="560d5-104">Az áttelepítési köteg kihagyott elemeinek jóváhagyása:</span><span class="sxs-lookup"><span data-stu-id="560d5-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="560d5-105">Set-MigrationBatch \<kötegnév> -ApproveSkipitems</span><span class="sxs-lookup"><span data-stu-id="560d5-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="560d5-106">A következő paranccsal hagyhatja jóvá a "Szinkronizált" de nem befejezett áttelepítési kérelmek kihagyott elemeit:</span><span class="sxs-lookup"><span data-stu-id="560d5-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="560d5-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkipedItemApprovalTime $([DateTime]::UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="560d5-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="560d5-108">Az áttelepítési köteg nek és a kérelmeknek néhány perc alatt újra kell kezdődnie és befejeződniük.</span><span class="sxs-lookup"><span data-stu-id="560d5-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

