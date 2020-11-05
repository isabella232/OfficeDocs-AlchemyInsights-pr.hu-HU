---
title: Azure számlázási tulajdonjog átvitele
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922077"
---
# <a name="transfer-azure-billing-ownership"></a>Azure számlázási tulajdonjog átvitele

Bejelentkezés az [Azure portálra](https://portal.azure.com/) az átvinni kívánt előfizetést tartalmazó számlázási fiók rendszergazdájától. Ha nem biztos abban, hogy Ön és rendszergazdája, vagy ha meg szeretné állapítani, hogy ki az, akkor olvassa el a [fiók számlázási rendszergazdájának meghatározása](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)című témakört.

- Keressen a **Cost Management + számlázás** lapon.
- Válassza a bal oldali ablaktábla **előfizetések** elemét. A hozzáféréstől függően előfordulhat, hogy ki kell választania egy számlázási hatókört, majd **előfizetéseket** vagy **Azure-előfizetéseket**.
- Válassza a **Számlázási tulajdonjog átruházása** lehetőséget az átvinni kívánt előfizetés esetén
- Adja meg egy olyan felhasználó e-mail-címét, aki számlázási rendszergazdája az előfizetés új tulajdonosa lesz, majd válassza az **átadás-összehívás küldése** lehetőséget.
- A felhasználó megkapja az átadási kérést ismertető e-mailt. Az átadás-összehívás jóváhagyásához a felhasználó kiválasztja a hivatkozást az e-mailben, és követi az útmutatást.

**Megjegyzés** : Ha az előfizetése számlázási tulajdonjogát egy másik Azure ad-bérlői fiókba ruházza át, az előfizetésben szereplő erőforrások kezeléséhez az összes [szerepkör-alapú hozzáférés-vezérlési (RBAC-)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)hozzárendelést véglegesen eltávolítja a rendszer. Az előfizetésben csak az új tulajdonos férhet hozzá az erőforrások kezeléséhez. További információ: [előfizetés átvitele egy másik Azure ad-bérlői fiókba](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Ajánlott dokumentumok**

- [Azure-előfizetés számlázási tulajdonjogának átvitele másik fiókba](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Az Azure-előfizetés számlázási tulajdonjogának átvitele](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [A Visual Studio, a Microsoft Partner Network (MPN) és a kifizetések átvitele a dev/próba-előfizetések segítségével](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Tulajdonosi kérdések átvitele](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Átvitel tulajdonjogával kapcsolatos problémák elhárítása](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
