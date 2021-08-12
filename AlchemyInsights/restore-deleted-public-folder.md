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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943377"
---
# <a name="restore-a-deleted-public-folder"></a>Törölt nyilvános mappa visszaállítása

**Törölt elemek visszaállítása nyilvános mappából:**

- Lásd: Nem lehet helyreállítani a törölt elemeket egy nem levelezési nyilvános mappából a [Outlook 2016.](https://aka.ms/pfrec)
 
**Törölt nyilvános mappa (bármilyen típusú)** visszaállítása: 

- Használja a következő EXO PowerShell-parancsot:

    Szintaxis:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Példa: A következő paranccsal visszaállíthatja az Almappa1 mappáját, és a \Parent1 mappába adhatja:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

További [részletekért lásd:](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) Törölt nyilvános mappa visszaállítása.
