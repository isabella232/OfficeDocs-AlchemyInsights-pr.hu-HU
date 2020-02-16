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
# <a name="restore-a-deleted-public-folder"></a>Törölt nyilvános mappa visszaállítása

**Törölt elemek visszaállítása nyilvános mappából:**

- Lásd: Nem lehet visszaállítani a [törölt elemeket egy nem e-mail nyilvános mappából az Outlook 2016-ban.](https://aka.ms/pfrec)
 
**Törölt (bármilyen típusú) nyilvános mappa visszaállítása:** 

- Használja a következő EXO PowerShell parancsot:

    Szintaxis:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Név -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Elérési út, ahol a mappa vissza lesz állítva>

    Példa: A következő parancs visszaállítja az Almappát1, és a \Parent1 alá helyezi:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Név -eq "Almappa1"}; Set-PublicFolder $pf.identity -Path \Parent1

További részletekért [lásd: Törölt nyilvános mappa visszaállítása.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
