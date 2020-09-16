---
title: Nyilvános mappa áttelepítési kötegének CompletedWithErrors állapotával
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
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744115"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Nyilvános mappa áttelepítési kötegének CompletedWithErrors állapotával

Az alábbi lépésekkel fejezheti be a köteget, és kihagyhatja a nagy/hibás elemeket: 
1. A kihagyott elemek jóváhagyása az áttelepítési kötegben:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. A következő paranccsal hagyja jóvá a kihagyott elemeket a szinkronizált, de nem befejezett áttelepítési kérelmekben:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Az áttelepítési kötegnek és a kéréseknek néhány percen belül el kell végezniük.

