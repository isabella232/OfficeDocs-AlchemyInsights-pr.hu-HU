---
title: Rendszergazdák hozzáadása és kezelése
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755497"
---
# <a name="how-to-add-and-manage-admins"></a>Rendszergazdák hozzáadása és kezelése

A probléma leírása alapján megtalálunk egy megoldást. A legtöbb ügyfél saját maga oldhatja fel a problémát a dokumentációt követően.

A Microsoft Customer Agreement (MCA) számlázási fiókjának kezeléséhez eltérő szerepköröket használhat az Access kívánt szintjéhez. Ezek a szerepkörök az Azure rendszer beépített szerepköreit is magukban foglalják, amelyek segítik az erőforrások irányítását.

**Számlázási Szerepkörök hozzáadása az Azure portálon:**

1. Bejelentkezés az [Azure portálra](https://portal.azure.com/)
2. Keressen a *Cost Management + számlázás* lapra.
3. Válassza a hozzáférés-vezérlés (IAM) lehetőséget olyan hatókörben, mint például a Számlázási fiók, a számlázási profil vagy a számla szakasz, ahol hozzáférést szeretne adni.
4. A hozzáférés-vezérlés (IAM) lap felsorolja azokat a felhasználókat és csoportokat, amelyek az adott hatókörhöz tartozó egyes szerepkörökhöz vannak rendelve.
5. Ha hozzáférést szeretne adni egy felhasználóhoz, válassza a lap tetején a **Hozzáadás** lehetőséget. A *szerepkör* legördülő listában válasszon egy szerepkört. Adja meg annak a felhasználónak az e-mail-címét, akinek hozzáférést szeretne adni. A szerepkör hozzárendeléséhez válassza a **Mentés** gombot.
6. Ha el szeretné távolítani a hozzáférést egy felhasználóhoz, jelölje ki azt a felhasználót, akivel el szeretné távolítani az eltávolítandó szerepkör-feladatot. Kattintson az **Eltávolítás** gombra.

**Ajánlott dokumentumok**

- [Számlázási szerepkör-definíciók](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [Számlázási fiók – szerepkörök és feladatok](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [Első lépések az MCA számlázási fiókjával](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [Microsoft-ügyfél-szerződéshez való hozzáférés ellenőrzése](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
