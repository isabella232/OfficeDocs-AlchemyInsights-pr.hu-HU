---
title: Támogatott előfizetési típusok
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807564"
---
# <a name="supported-subscription-types"></a>Támogatott előfizetési típusok

Kérjük, tekintse át a támogatott előfizetési típusokat a további folytatáshoz.

[Támogatott előfizetési típusok](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Számlázási tulajdonjog átruházása**

Azure Portal – az átvinni kívánt előfizetést tartalmazó számlázási fiók [rendszergazdája](https://ms.portal.azure.com/)

- Keressen a **Cost Management + számlázás** lapon. Válassza a bal oldali ablaktábla **előfizetések** elemét. A hozzáféréstől függően előfordulhat, hogy ki kell választania egy számlázási hatókört, majd **előfizetéseket** vagy **Azure-előfizetéseket** .
- Válassza a számlázási tulajdonjog átruházása lehetőséget az átvinni kívánt előfizetés esetén
- Adja meg egy olyan felhasználó e-mail-címét, aki számlázási rendszergazdája az előfizetés új tulajdonosa lesz, majd válassza az **átadás-összehívás küldése** lehetőséget.
- A felhasználó megkapja az átadási kérést ismertető e-mailt. Az átadás-összehívás jóváhagyásához a felhasználó kiválasztja a hivatkozást az e-mailben, és követi az útmutatást.

Megjegyzés: Ha az előfizetése számlázási tulajdonjogát egy másik Azure AD-bérlői fiókba ruházza át, az előfizetésben szereplő erőforrások kezeléséhez az összes [szerepkör-alapú hozzáférés-vezérlési (RBAC-)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) hozzárendelést véglegesen eltávolítja a rendszer. Az előfizetésben csak az új tulajdonos férhet hozzá az erőforrások kezeléséhez. További információ: [előfizetés átvitele egy másik Azure ad-bérlői fiókba](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Az előfizetés tulajdonjogának átruházása**

Az előfizetés tulajdonosi átvitelének előfeltételei a role-based Access (RBAC) az előfizetésben lévő erőforrások kezeléséhez elvesztik a hozzáférést. Ha szeretne többet megtudni arról, hogy miként vehet fel meglévő előfizetést bérlői fiókba, olvassa el [Az Azure-előfizetés társítása vagy hozzáadása az Azure Active Directoryhoz](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)című témakört

- A meglévő számlázási ciklusból származó meglévő hátralékos előfizetés átvitele az új fiókba nem kerül át az új fizetési instrumentumba. Az új fiókba tartozó felhasználók számára elérhető egyetlen adat az előfizetés utolsó havi költsége. A többi használat és a számlázási előzmények nem adják át az előfizetést.
- A vállalati szerződési (EA) előfizetések számlázási tulajdonjogának átvitele jelenleg a nagyvállalati szerződés portálon érhető el.
- A kredit-orientált előfizetések, például a Visual Studio, a BizSpark, a Microsoft partner hálózat új felhasználóknak való átviteléhez Visual Studio/Microsoft partner hálózati licenccel kell rendelkeznie az átadás-összehívás elfogadásához.
- Minden erőforrás, például a virtuális gépek, a lemezek és a webhelyek sikeres átadása az új fiókba. A következő erőforrásokat érintheti a több bérlői előfizetés átvitele:

**Azure AD Domain Services**

Azure fő pince-tárolók

- Az SQL-alapú [kapcsolódó felhasználók és adatbázisok](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) hatással lehetnek, különösen akkor, ha az ügyfél Azure Active Directory-alapú hitelesítést használ
- Az Azure Active Directory-hitelesítéssel konfigurált **app-szolgáltatások** hatással lehetnek
- **Visual Studio-csapat** Az Azure-előfizetésekhez kapcsolódó szolgáltatások átmenetileg elveszíthetik az Accessben, amikor a csatlakoztatott Azure-előfizetés meg van szakítva

**Ajánlott dokumentumok**

A számlázási tulajdonjog elfogadása után elvégzendő lépések:

- Ha meg szeretné őrizni a számlázási tulajdonjogot, de módosítani szeretné az előfizetését, olvassa el a következő témakört: [Az Azure-előfizetés váltása másik ajánlatra](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A Visual Studio, a Microsoft Partner Network (MPN) és a kifizetések átvitele a dev/próba-előfizetések segítségével](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [A vállalati szerződés (EA) előfizetések számlázási tulajdonjogának átvitele](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Tulajdonosi kérdések átvitele](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Átvitel tulajdonjogával kapcsolatos problémák elhárítása](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)