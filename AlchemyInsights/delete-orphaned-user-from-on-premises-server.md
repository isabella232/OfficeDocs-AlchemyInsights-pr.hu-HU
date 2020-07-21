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
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="746f8-102">Árva felhasználó törlése a helyszíni kiszolgálóról</span><span class="sxs-lookup"><span data-stu-id="746f8-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="746f8-103">Árva felhasználó eltávolításához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="746f8-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="746f8-104">Címtár-szinkronizálás kényszerítése a Mi a [hibrid identitás az Azure Active Directoryval című](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)könyv utasításait követve.</span><span class="sxs-lookup"><span data-stu-id="746f8-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="746f8-105">A címtár-szinkronizálás ellenőrzéséhez olvassa el [a Mi a hibrid identitás az Azure Active Directoryval?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="746f8-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="746f8-106">Ha a szinkronizálás megfelelően működik, de az Active Directory-objektum törlése nem terjed az Azure AD-re, manuálisan távolítsa el az árva objektumot az alábbi Azure Active Directory-modul windows PowerShell-parancsmagok használatával:</span><span class="sxs-lookup"><span data-stu-id="746f8-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="746f8-107">Eltávolítás-MsolContact</span><span class="sxs-lookup"><span data-stu-id="746f8-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="746f8-108">Eltávolítás-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="746f8-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="746f8-109">Eltávolítás-MsolUser</span><span class="sxs-lookup"><span data-stu-id="746f8-109">Remove-MsolUser</span></span>

    <span data-ttu-id="746f8-110">Ha például el szeretné távolítani az elárvult felhasználói azonosítót john.smith@contoso.com, amelyet eredetileg a címtár-szinkronizálással hoztak létre, futtassa a parancsmabát:</span><span class="sxs-lookup"><span data-stu-id="746f8-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="746f8-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="746f8-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>