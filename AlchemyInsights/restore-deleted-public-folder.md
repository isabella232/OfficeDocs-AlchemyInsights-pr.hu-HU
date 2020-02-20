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
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158506"
---
# <a name="restore-a-deleted-public-folder"></a>Törölt nyilvános mappa visszaállítása

**Törölt elemek visszaállítása nyilvános mappából:**

- Lásd: Nem lehet visszaállítani a [törölt elemeket egy nem e-mail nyilvános mappából az Outlook 2016-ban.](https://aka.ms/pfrec)
 
**Törölt (bármilyen típusú) nyilvános mappa visszaállítása:** 

- Használja a következő EXO PowerShell parancsot:

    Szintaxis:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Példa: A következő parancs visszaállítja az Almappát1, és a \Parent1 alá helyezi:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

További részletekért [lásd: Törölt nyilvános mappa visszaállítása.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
