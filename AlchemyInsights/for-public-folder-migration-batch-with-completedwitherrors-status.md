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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Befejezett hiba állapotú nyilvános mappa áttelepítési köteg esetén

A köteg befejezéséhez kövesse az alábbi lépéseket, kihagyva a nagy/rossz elemeket: 
1. Az áttelepítési köteg kihagyott elemeinek jóváhagyása:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. A következő paranccsal hagyhatja jóvá a "Szinkronizált" de nem befejezett áttelepítési kérelmek kihagyott elemeit:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Az áttelepítési köteg nek és a kérelmeknek néhány perc alatt újra kell kezdődnie és befejeződniük.

