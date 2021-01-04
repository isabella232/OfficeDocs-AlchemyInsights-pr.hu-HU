---
title: Azure-előfizetés számlázási tulajdonjogának átadása
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
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736880"
---
# <a name="transfer-azure-billing-ownership"></a>Azure-előfizetés számlázási tulajdonjogának átadása

Jelentkezzen be a [Microsoft Azure Portalra](https://portal.azure.com/) az átvinni kívánt előfizetéssel rendelkező számlázási fiók rendszergazdájaként. Ha nem biztos abban, hogy Ön a rendszergazda, vagy meg szeretné állapítani, hogy ki az, olvassa el a [Fiók számlázási rendszergazdájának megállapítása](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa) című témakört.

1. Keressen a _Költségkezelés + számlázás_ elemre.
1. Válassza a bal oldali ablaktábla **Előfizetések** elemét. A hozzáféréstől függően előfordulhat, hogy ki kell választania egy számlázási hatókört, majd az **Előfizetések** vagy az **Azure-előfizetések** lehetőséget.
1. Az átvinni kívánt előfizetésnél válassza ki a **Számlázási tulajdonjog átadása** lehetőséget.
1. Írja be azon fiók számlázási rendszergazdájának az e-mail-címét, aki az átadni kívánt előfizetés új tulajdonosa lesz, majd válassza az **átadási kérelem küldése** lehetőséget.
1. A felhasználó kap egy utasításokat tartalmazó e-mailt az átadási kérelem áttekintéséhez. Az átadási kérelem jóváhagyásához a felhasználó kiválasztja az e-mailben található hivatkozást, és követi az utasításokat.

Felhívjuk a figyelmét arra, hogy ha az előfizetése számlázását egy másik Azure AD-bérlői fiókban található felhasználói fiókra ruházza át, az előfizetésben lévő erőforrások kezelésére vonatkozó összes [szerepköralapú hozzáférés-vezérlési (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) hozzárendelést véglegesen törli a rendszer. Az előfizetés erőforrásainak kezelésére csak az új tulajdonos lesz jogosult. Az előfizetések címtárának módosításáról további információt az [Előfizetés áthelyezése egy másik Azure AD-bérlői fiókba](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support) című témakörben talál.

_**A számlázást érintő fontos tényező**_: Ha egy Azure-előfizetés számlázását adta át, a díjak arányosítva lesznek. A számlákat az alábbiak szerint érheti el:  

1. Válassza ki az előfizetését az [Előfizetések lapról](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) az Azure Portal felületén [egy olyan felhasználói fiókkal, amelyik hozzáféréssel rendelkezik a számlákhoz](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), majd válassza a **számlák** lehetőséget.
1. A PDF-számla egy példányának megtekintéséhez kattintson a  **Számla letöltése**  gombra. Ha a _Nem érhető el_ üzenet jelenik meg, tanulmányozza a következő témakört: [Miért nem jelenik meg a legutóbbi számlázási időszakra vonatkozó számla?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. A napi használatot úgy is megtekintheti, ha a **számlázási időszakra** kattint, amellyel hozzájut a számlája egy PDF-formátumú példányához, valamint a részletes napi használatot tartalmazó fájlhoz (.CSV). További információ: [Számlázási és használati adatok lekérése](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Ajánlott dokumentumok**

- [Azure-előfizetés számlázási tulajdonjogának átadása másik fióknak](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Az Azure-előfizetés számlázási tulajdonjogának átadása](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [A Visual Studio-, a Microsoft Partner Network- (MPN-) és a használatalapú fizetési móddal rendelkező Dev/Test-előfizetések átadása](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [A tulajdonjog átadásával kapcsolatos gyakori kérdések (GYIK)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [A tulajdonjog átadásával kapcsolatos hibaelhárítás](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
