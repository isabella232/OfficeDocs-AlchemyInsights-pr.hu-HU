---
title: Áttelepítés AIP-ről MIP-re/egyesített címkézésre a Megfelelőségi központban
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000358"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Áttelepítés AIP-ről MIP-re/egyesített címkézésre a Megfelelőségi központban

Az AIP-címkékről az Egyesített címkézésre való áttelepítéshez a Biztonsági és megfelelőségi központban tegye a következőket:

**Az Azure Portal védelmének aktiválása**

1. Ha még nem tette meg, nyisson meg egy új böngészőablakot, és jelentkezzen be [az Azure Portalba.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Lépjen az **Azure Information Protection blade (Azure Information Protection) lapra.** A központ menüben például  kattintson a Minden  szolgáltatás elemre, és kezdje el beírni az Információ szöveget a Szűrő mezőbe. Válassza az **Azure Information Protection (Azure Information Protection) lehetőséget.** Ha még nem fért hozzá az Azure Information Protection [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) blade-hez, tekintse meg a blade felvételének egyszeres további lépéseit a portálra. Az Azure Information Protection blade megnyitásához [Azure Information Protection](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) Prémium vagy egy rights managementet tartalmazó Office 365 kell lennie. Ha rendelkezik az alábbi előfizetések egyikével, de üzenet jelenik meg arról, hogy nem található érvényes előfizetés, forduljon a [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ügyfélszolgálatához, vagy használja a szokásos támogatási csatornákat.

2. Keresse meg **a Kezelés** menü beállításait, és válassza a **Védelem aktiválása lehetőséget.** Kattintson **az Aktiválás** gombra, majd erősítse meg a műveletet. Ha befejeződött az aktiválás, az információs sávon megjelenik **az Aktiválás sikeresen befejeződött üzenet.**

**Azure Information Protection-címkék áttelepítése Office 365 Biztonsági & megfelelőségi központba**

1. Győződjön meg arról, hogy globális rendszergazdai engedéllyel rendelkező felhasználóként jelentkezett be.

2. Lépjen az **Azure Information Protection blade (Azure Information Protection) lapra.**

3. A Kezelés **menüben** válassza az **Egységes címke lehetőséget.**

4. Az **Azure Information Protection – Egységes** címkével jelölt címkeszálon kattintson az Aktiválás elemre, **és** kövesse az online utasításokat.

**Megjegyzés:** Ellenőrizze, hogy rendelkezik-e a megfelelő engedélyekkel a Biztonsági központ & áttelepítése előtt. További információt az alábbi cikkekben talál:

1. [Az Azure Information Protection konfigurálhoz globális rendszergazdának kell lennie, vagy más rendszergazdáknak kell delegálnom?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Fontos információk a felügyeleti szerepkörökről a Biztonsági és megfelelőségi központba & után.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Az AIP to Unified Labeling migration to Security and [](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)Compliance Center (AIP – Egységes címkézés migrálás a Biztonsági és megfelelőségi központba) eszközről további információt a Címkék áttelepítésecímkebe.
