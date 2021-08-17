---
title: A számla vagy a használat másolatára van szükség
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
- "9003801"
- "6804"
ms.openlocfilehash: ea300839f840110f65c3ce51899c89f96294202595b3933d411d6f1803fa7e43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116910"
---
# <a name="get-a-copy-of-your-bill-or-usage"></a>A számla vagy a használat másolatának lekérte

**Az Azure-számla (.pdf) letöltése**

1. Válassza ki az előfizetését az [Előfizetések lapon](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) az Azure Portal felületén [egy olyan felhasználói fiókkal, amelyik hozzáféréssel rendelkezik a számlákhoz](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), majd válassza a **Számlák** lehetőséget.
2. A PDF-számla egy példányának megtekintéséhez kattintson a **Számla letöltése** gombra. Ha a **Nem érhető el** üzenet jelenik meg, tanulmányozza a következő cikket:[Miért nem jelenik meg a legutóbbi számlázási időszakra vonatkozó számla?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
3. A napi használatot úgy is megtekintheti, ha a számlázási időszakra kattint, amellyel hozzájut a számlája egy PDF-formátumú példányához, valamint a részletes napi használatot tartalmazó fájlhoz (.CSV): [Számlázási és használati adatok lekérése](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)

**Számla lekérte e-mailben (.pdf)**

1. Válassza ki előfizetését az [Előfizetések lapon.](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Kattintson **a Számlák, majd** a Saját számla küldése **e-mailben elemre.**
2. Kattintson **az opt in (opt in) gombra,** és fogadja el a feltételeket. Minden előfizetéséhez külön-külön be kell jelentkeznie. Megjegyzés: Ha a lépések után nem kap e-mailt, ellenőrizze, hogy helyes-e az e-mail-cím a profil kommunikációs [beállításai között](https://account.windowsazure.com/profile)
3. [A Beérkezett üzenetek mappába e-mailben küldött Azure-számlák](https://azure.microsoft.com/blog/azure-email-invoices/)

**A napi használat megérti:**  
 [A számlázási számla Microsoft Azure](https://docs.microsoft.com/azure/cost-management-billing/understand/review-individual-bill?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Költségek kezelése:** [Váratlan költségek megelőzése az Azure számlázásával és költségkezelésével](https://docs.microsoft.com/azure/cost-management-billing/manage/getting-started?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Microsoft ügyfélszerződés (MCA):**

[Megtudhatja, hogyan ellenőrizheti a Microsoft ügyfélszerződéshez való hozzáférését?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)  
Ha microsoftos ügyfélszerződése [van,](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)a használatot az [Azure Portal webhelyen töltheti le.](https://portal.azure.com/)

**A Microsoft ügyfélszerződésében szereplő számlák e-mailben való lekérte:**

Ha microsoftos ügyfélszerződése van, a számláját e-mailben lekértheti. Minden számlázási profil: Tulajdonosok, Közreműködők, Olvasók és Számlakezelők e-mailben kapják meg a számlát. Az olvasók nem tudják frissíteni az e-mailben szereplő számla beállítását

- Keresse meg a **Költségkezelés + számlázás** elemet. Válasszon ki **egy számlázási profilt.** A Beállítások Gépház válassza a Tulajdonságok **lehetőséget.**
- Az E-mail-számla alatt válassza az **E-mail-számla beállításának frissítése lehetőséget.** Válassza az Opt in (Opt in) lehetőséget. Kattintson a **Frissítés gombra.**

**Nagyvállalati Szerződés (EA)**

A használati adatok EA-ügyfélként való megtekintéséhez és letöltéséhez nagyvállalati rendszergazdának, fióktulajdonosnak vagy részleg-rendszergazdának kell lennie, akinél engedélyezve van a díjletöltési házirend.

- Jelentkezzen be az Azure portálra. Keresse meg a **Költségkezelés + számlázás** elemet. Számlázási profil kiválasztása
- Válassza a Usage +charges (Használat + díjak) lehetőséget. A letölteni kívánt hónaphoz válassza a Letöltés lehetőséget.

**MOSP Azure-előfizetés**  
[MOSP Azure-előfizetési számla letöltése](https://docs.microsoft.com/azure/cost-management-billing/understand/download-azure-invoice?WT.mc_id=Portal-Microsoft_Azure_Support#download-your-mosp-azure-subscription-invoice)

**Hibaelhárítás: Nem látható a legutóbbi számlázási időszak számlája?**

Néhány lehetséges ok, amiért esetleg nem látható a számla:

- Olyan havi kreditet kap az előfizetésével, amely nem lépte túl, vagy ingyenes próbaverzióval rendelkezik. Egy számla csak akkor jön létre, ha Ön tartozásból
- Kevesebb mint 30 nap van attól a naptól, amikor előfizetett az Azure-ra.
- A számla még nem jön létre. Várakozás a számlázási időszak végéig
- Ha Ön nem ügyfél-rendszergazda, előfordulhat, hogy a régebbi számlák nem érhetők el az Ön számára **Megjegyzés:** A Microsoft nem nyújt használati jelentéseket vagy használati adatokat az Azure felhőszolgáltató ügyfeleinek. A Partnerközpont használati adatai partnerrel kapcsolatban áll
- További információ az AIO (Azure in open) számlázásról és használatról: [Azure in open](https://azure.microsoft.com/offers/ms-azr-0111p/)

**Ajánlott dokumentumok**

- [Miért nem látható egy számla?](https://docs.microsoft.com/azure/cost-management-billing/understand/download-azure-invoice?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
- [Azure számlázási számla és használati adatok kérése/letöltése/megtekintése](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure-számlák küldése közvetlenül a Beérkezett üzenetek mappába](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Részletes használati díjak](https://docs.microsoft.com/azure/cost-management-billing/understand/review-individual-bill?WT.mc_id=Portal-Microsoft_Azure_Support#csv)
- [A számlán szereplő feltételek](https://docs.microsoft.com/azure/cost-management-billing/understand/understand-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure felhőszolgáltatói számla](https://docs.microsoft.com/partner-center/azure-plan-lp?WT.mc_id=Portal-Microsoft_Azure_Support)
