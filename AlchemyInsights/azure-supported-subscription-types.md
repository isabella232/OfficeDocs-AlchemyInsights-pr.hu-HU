---
title: Támogatott előfizetéstípusok
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072162"
---
# <a name="supported-subscription-types"></a>Támogatott előfizetéstípusok

A folytatáshoz tekintse át a támogatott előfizetéstípusokat.

[Támogatott előfizetéstípusok](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**A számlázás tulajdonjogának átruházása**

Azure Portal, [mint](https://ms.portal.azure.com/) az át átruházni kívánt előfizetéshez szükséges számlázási fiók fiók rendszergazdája

- Keressen a **Költségkezelés + számlázás** elemre. Válassza **az Előfizetések** lehetőséget a bal oldali ablaktáblában. A hozzáféréstől függően előfordulhat, hogy ki kell választania egy számlázási hatókört, majd az **Előfizetések** vagy az **Azure-előfizetések** lehetőséget.
- Válassza az át átruházni kívánt előfizetés számlázási tulajdonosának átvitele lehetőséget.
- Adja meg annak a felhasználónak az e-mail-címét, aki az előfizetés új tulajdonosa lesz a fiók számlázási **rendszergazdája,** majd válassza az átviteli kérelem küldése lehetőséget.
- A felhasználó kap egy utasításokat tartalmazó e-mailt az átadási kérelem áttekintéséhez. Az átadási kérelem jóváhagyásához a felhasználó kiválasztja az e-mailben található hivatkozást, és követi az utasításokat.

Megjegyzés: Ha egy másik Azure AD-bérlő felhasználói fiókjához irányítja át az előfizetés számlázási tulajdonjogát, a [szerepköralapú hozzáférés-vezérlési (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) hozzárendelések végleg törlődnek az előfizetés erőforrásainak kezeléséhez. Az előfizetés erőforrásainak kezelésére csak az új tulajdonos lesz jogosult. További információ: Előfizetés átvitele egy másik [Azure AD-bérlő felhasználónak.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**Előfizetés tulajdonjogának átruházása**

Az előfizetés tulajdonjogának átruházása előfeltételei a szerepköralapú hozzáférésnek (RBAC) az előfizetés erőforrásainak kezeléséhez. Ha többet szeretne tudni arról, hogy hogyan adhat hozzá meglévő előfizetést egy bérlőhöz, tekintse meg az Azure-előfizetés társítása vagy hozzáadása a bérlőhöz [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

- Az aktuális számlázási ciklusban már fennálló fennálló összeggel fennálló előfizetés-átvitel nem kerül át az új fiók új fizetési eszközére. Az új fiók felhasználói számára csak az előfizetése utolsó havi költsége áll rendelkezésre. A használati és számlázási előzmények többi része nem kerül át az előfizetésbe.
- Az Nagyvállalati Szerződés (EA) előfizetések számlázási tulajdonjogának átvitele jelenleg csak az Nagyvállalati Szerződés portálon támogatott
- A hitelorientált előfizetések (például Visual Studio, BizSpark, Microsoft Partner Network) új felhasználónak való átviteléhez Visual Studio/Microsoft-partnerhálózati licenc szükséges az átviteli kérelem elfogadásához
- Minden erőforrás, például virtuális gépek, lemezek és webhelyek sikeresen átküldve az új fiókba. A bérlők közötti előfizetés-átvitel az alábbi erőforrásokat érintheti:

**Azure AD tartományi szolgáltatások**

Azure-kulcst tárolók

- [SQL felhasználókra](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) és adatbázisokra is hatással lehet, különösen akkor, ha az ügyfél Azure Active Directory hitelesítést használ.
- **Hatással lehet** a Azure Active Directory konfigurált appszolgáltatásokra.
- **Visual Studio csapat** Az Azure-előfizetésekkel összekapcsolt szolgáltatások fiókjai átmenetileg megszűnhetnek a hozzáférésük a csatlakoztatott Azure-előfizetés lemondása esetén

**Ajánlott dokumentumok**

A számlázási tulajdonjog elfogadásának lépései:

- Ha meg kell tartania a számlázási tulajdonjogot, de meg kell változtatnia az előfizetés típusát, olvassa el a következőt: [Azure-előfizetés váltása másik ajánlatra](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A Visual Studio-, a Microsoft Partner Network- (MPN-) és a használatalapú fizetési móddal rendelkező Dev/Test-előfizetések átadása](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Előfizetések számlázási tulajdonjogának Nagyvállalati Szerződés (EA) előfizetések esetén](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [A tulajdonjog átadásával kapcsolatos gyakori kérdések (GYIK)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [A tulajdonjog átadásával kapcsolatos hibaelhárítás](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)