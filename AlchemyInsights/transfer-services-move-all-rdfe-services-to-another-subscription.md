---
title: Átviteli szolgáltatások – az összes RDFE-szolgáltatás áthelyezése másik előfizetésbe
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692045"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Átviteli szolgáltatások – az összes RDFE-szolgáltatás áthelyezése másik előfizetésbe

**Erőforrások áthelyezése**

Az Azure-erőforrásokat az Azure Portal, az Azure PowerShell, az Azure CLI vagy a REST API segítségével áthelyezheti egy másik Azure-előfizetésbe vagy erőforrás-csoportba az erőforrások áthelyezéséhez.

Az erőforrások áthelyezése előtt az alábbiakra van lehetősége:

- [Ellenőrzőlista az erőforrások áthelyezése előtt](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Áthelyezhető szolgáltatások](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Az áthelyezés érvényesítése](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Útmutatás áthelyezése a szolgáltatásokhoz](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Ha a meglévő erőforrásokat át szeretné helyezni egy másik erőforráscsoporthoz vagy előfizetésbe, az alábbiakat használhatja:

- [Azure-portál](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Oktatóanyag: [Az Azure-erőforrások áthelyezése másik erőforrás-csoportba vagy-előfizetésbe](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Az Azure Resource Manager hibáinak elhárítása**

Az alábbi cikkekből megtudhatja, hogy miként találhatja meg az Azure néhány gyakori központi telepítési hibáját, és hogyan kaphat információt a megoldásához. Ha nem találja a központi telepítő hibájának megfelelő hibakódot, olvassa el a [hibakód keresése](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)című témakört.

- [A központi telepítő hibáinak elhárítása](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Azure-erőforrások új erőforráscsoporthoz vagy előfizetésbe való áthelyezésével kapcsolatos hibák elhárítása](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Felhívjuk a figyelmét arra, hogy ha frissíteni szeretné az Azure-előfizetését, például az ingyenes fizetésről a befizetésre, az előfizetést konvertálnia kell.

- Ha frissíteni szeretne egy ingyenes próbaverziót, olvassa el [az ingyenes próbaverzió frissítése vagy a Microsoft Imagine Azure-előfizetés a fizetéshez](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Ha egy fizetési mód szerinti fizetési módot szeretné módosítani, olvassa el az [Azure Pay-as-your-go-előfizetés módosítása másik ajánlatra](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)című témakört.

**Azure-előfizetés hozzáadása vagy társítása az Azure Active Directory-bérlői webhelyhez:**

1. Bejelentkezés, és válassza ki a használni kívánt előfizetést az [Azure Portal előfizetések lapjáról](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Válassza a **címtár módosítása** elemet.
3. Ellenőrizze a megjelenő figyelmeztetéseket, majd kattintson a **módosítás** gombra.
4. Az előfizetés megváltoztatja a címtárat, és sikerről szóló üzenetet kap.
5. Nyissa meg az új könyvtárat a *címtár* -kapcsoló használatával. Akár 10 percet is igénybe vehet, hogy minden megfelelően megjelenjen.

**Ajánlott dokumentumok**

- [Azure-előfizetés tulajdonjogának átvitele](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Erőforrások áthelyezése új erőforrás-csoportba vagy előfizetésbe](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Erőforrások kezelése az Azure Portal segítségével](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
