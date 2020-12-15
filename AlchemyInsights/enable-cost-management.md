---
title: A költség-kezelés engedélyezése
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677737"
---
# <a name="enable-cost-management"></a>A költség-kezelés engedélyezése

**Mit jelent az, hogy a költségek le vannak tiltva a szervezetében?**

A vállalati szerződéssel (EA) vagy a Microsoft Customer Agreement (MCA) fiókkal rendelkező szervezetek a költség-és árképzési adatokhoz való hozzáférést is letilthatják.

Miután bejelentkezett az Azure portálra, a számlázási API-k segítségével programozott módon beolvashatja a számlákat (ha nincs bekapcsolva) és a használati adatait.

**A számlák elérésének engedélyezése további felhasználóknak**

1. Nyissa meg az **előfizetések lapátot** az Azure portálon.
2. Válassza a **számlák** , majd **a számlákhoz való hozzáférést**.
3. Kapcsolja be a hozzáférést, majd a módosítások mentését követően engedélyezze, hogy a felhasználók előfizetéssel kapcsolatos hatókörű szerepköröket töltsenek le a számlák letöltéséhez.

> [!NOTE]
> A fiók rendszergazdája úgy is beállíthatja, hogy a számlák e-mailen keresztül legyenek elküldve. További információt a [számla beszerzése e-mailben](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)című témakörben találhat.

**Felhasználók felvétele a számlázási olvasó szerepkörbe**

1. Nyissa meg az **előfizetések lapátot** az Azure portálon.
2. Válassza a **hozzáférés-vezérlés (iam)** lehetőséget, majd kattintson a **Hozzáadás** gombra.
3. Válassza a **Számlázási olvasó** lehetőséget a **szerepkör kiválasztása** lapon.
4. Írja be a meghívni kívánt felhasználó e-mail-címét, majd az **OK** gombra kattintva küldje el a meghívót.
5. Kövesse az e-mailek meghívása számlázási olvasóként való bejelentkezéshez című témakör utasításait. További információt a [hozzáférés biztosítása a számlázáshoz](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)című témakörben talál.

**Ajánlott dokumentumok**

- [A DA és az AO nézet engedélyezése az EA portálon keresztül](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [A Cost-kezelés költségei](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Támogatott Microsoft Azure-ajánlatok](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [A költség-elemzés költségeinek áttekintése](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Hozzáférés biztosítása a számlázási adatokhoz](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Microsoft-ügyfél-szerződéshez való hozzáférés ellenőrzése](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






