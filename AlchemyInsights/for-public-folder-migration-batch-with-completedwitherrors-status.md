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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Befejezett hiba állapotú nyilvános mappa áttelepítési köteg esetén

A köteg befejezéséhez kövesse az alábbi lépéseket, kihagyva a nagy/rossz elemeket: 
1. Az áttelepítési köteg kihagyott elemeinek jóváhagyása:

    Set-MigrationBatch \<kötegnév> -ApproveSkipitems 
2. A következő paranccsal hagyhatja jóvá a "Szinkronizált" de nem befejezett áttelepítési kérelmek kihagyott elemeit:

    $pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkipedItemApprovalTime $([DateTime]::UtcNow)}}
3. Az áttelepítési köteg nek és a kérelmeknek néhány perc alatt újra kell kezdődnie és befejeződniük.

