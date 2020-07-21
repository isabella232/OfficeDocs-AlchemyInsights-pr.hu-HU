---
title: Árva felhasználó törlése a helyszíni kiszolgálóról
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198183"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Árva felhasználó törlése a helyszíni kiszolgálóról

Árva felhasználó eltávolításához kövesse az alábbi lépéseket:

1. Címtár-szinkronizálás kényszerítése a Mi a [hibrid identitás az Azure Active Directoryval című](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)könyv utasításait követve.

2. A címtár-szinkronizálás ellenőrzéséhez olvassa el [a Mi a hibrid identitás az Azure Active Directoryval?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ha a szinkronizálás megfelelően működik, de az Active Directory-objektum törlése nem terjed az Azure AD-re, manuálisan távolítsa el az árva objektumot az alábbi Azure Active Directory-modul windows PowerShell-parancsmagok használatával:

    Eltávolítás-MsolContact  
    Eltávolítás-MsolGroup  
    Eltávolítás-MsolUser

    Ha például el szeretné távolítani az elárvult felhasználói azonosítót john.smith@contoso.com, amelyet eredetileg a címtár-szinkronizálással hoztak létre, futtassa a parancsmabát:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com