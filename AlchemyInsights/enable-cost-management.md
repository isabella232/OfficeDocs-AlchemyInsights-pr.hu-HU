---
title: Költségkezelés engedélyezése
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
ms.openlocfilehash: 62f3cfb161c4f8da735bd288a2d6e22971b4aada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325465"
---
# <a name="enable-cost-management"></a>Költségkezelés engedélyezése

**Mit jelent az, hogy "a költségek le vannak tiltva a szervezet számára"?**

A Nagyvállalati Szerződés (EA) vagy a Microsoft Ügyfélszerződés (MCA) fiókját használó szervezetek letilthatják a hozzáférést a költséginformációkhoz és az árakkal kapcsolatos információkhoz.

Miután bejelentkezett az Azure Portalra, a számlázási API-k segítségével programozással leküldheti a számlákat (miután ezt választotta) és a használati adatokat.

**A számlákhoz való hozzáférés engedélyezése további felhasználóknak**

1. Az Azure **Portalon az Előfizetések blade lehetőséget** kell látnia.
2. Válassza **a Számlák,** majd a **Hozzáférés a számlákhoz lehetőséget.**
3. Kapcsolja be a hozzáférést, majd mentse a módosításokat, hogy az előfizetés-hatókörű szerepköröket használó felhasználók letöltsék a számlákat.

**Megjegyzés:** A fiók rendszergazdája beállíthatja azt is, hogy a számlákat e-mailben küldje el. További információt A számla lekérte [e-mailben.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**Felhasználók felvétele a Számlázási olvasó szerepkörbe**

1. Az Azure **Portalon az Előfizetések blade lehetőséget** kell látnia.
2. Válassza **a Hozzáférés-vezérlés (IAM) lehetőséget,** majd kattintson a Hozzáadás **gombra.**
3. Válassza **a Számlázási olvasó** lehetőséget a Szerepkör kiválasztása **lapon.**
4. Írja be a meghívni kívánt felhasználó e-mail-címét, majd az **OK** gombra kattintva küldje el a meghívót.
5. A számlázási olvasóként való bejelentkezéshez kövesse a meghívó e-mailben megadott utasításokat. További információ: [Hozzáférés megadása számlázáshoz.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)

**Ajánlott dokumentumok**

- [A DA és az AO nézet engedélyezése az EA portálon keresztül](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Költségkezelésben szereplő költségek](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Támogatott Microsoft Azure ajánlatok](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Költségek áttekintése a költségelemzésben](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Hozzáférés a számlázási adatokhoz](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A Microsoft ügyfélszerződéshez való hozzáférés ellenőrzése](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






