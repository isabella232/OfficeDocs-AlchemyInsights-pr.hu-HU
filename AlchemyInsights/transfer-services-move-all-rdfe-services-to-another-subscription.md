---
title: Szolgáltatások átvitele – Az összes RDFE-szolgáltatás áthelyezése egy másik előfizetésbe
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940060"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Szolgáltatások átvitele – Az összes RDFE-szolgáltatás áthelyezése egy másik előfizetésbe

**Erőforrások áthelyezése**

Az Azure-erőforrások áthelyezhetőek ugyanazon előfizetésen belül egy másik Azure-előfizetésbe vagy erőforráscsoportba az Azure Portal, az Azure PowerShell, az Azure CLI vagy a REST API használatával az erőforrások áthelyezéséhez.

Mielőtt áthelyezheti az erőforrásokat, tekintse át a következő forrásokat:

- [Ellenőrzőlista az erőforrások áthelyezését megelőzően](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Áthelyezhet szolgáltatásokat](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Az áthelyezés ellenőrzése](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Útmutató áthelyezése a szolgáltatásokhoz](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

A meglévő erőforrások másik erőforráscsoportba vagy előfizetésbe való áthelyezéséhez a következőt használhatja:

- [Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Oktatóprogram: [Azure-erőforrások áthelyezése másik erőforráscsoportba vagy -előfizetésbe](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Az Azure Resource Managerrel kapcsolatos hibák elhárítása**

Az alábbi cikkekből megismerhat néhány gyakori Azure-telepítési hibát, és információkat kaphat a megoldásukhoz. Ha nem találja a telepítési hibához szükséges hibakódot, tekintse meg a [Hibakód megkeresi a következőt:](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Telepítési hibák elhárítása](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Azure-erőforrások új erőforráscsoportba vagy -előfizetésbe való áthelyezésével kapcsolatos hibák elhárítása](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Felhívjuk a figyelmét arra, hogy ha frissíteni szeretné Azure-előfizetését, például az ingyenes előfizetésről a "fizetés"-előfizetésre szeretne váltani, át kell alakítania az előfizetését.

- Az ingyenes próbaverzió frissítéséhez tekintse meg Az ingyenes próbaverzió frissítése vagy a Microsoft Imagine Azure-előfizetésének frissítése ["Fizessen használatra" lehetőséget.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Ha másik fizetési fiókot módosítanának, tekintse meg Az Azure"-előfizetés módosítása másik ajánlatra " (Azure [Pay-As-You-Go) előfizetését.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Azure-előfizetés hozzáadása vagy társítása a Azure Active Directory bérlői fiókhoz:**

1. Jelentkezzen be, és válassza ki a használni kívánt előfizetést az [Azure Portal Előfizetések lapján.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Válassza **a Címtár módosítása lehetőséget.**
3. Tekintse át a megjelenő figyelmeztetéseket, és válassza a Módosítás **gombot.**
4. Az előfizetéshez módosult a címtár, és egy sikeres üzenetet kap.
5. A *Címtár-kapcsolóval* az új címtárra válthat. Akár 10 perc is elehet, hogy minden megfelelően mutasson.

**Ajánlott dokumentumok**

- [Azure-előfizetés tulajdonjogának átvitele](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Erőforrások áthelyezése új erőforráscsoportba vagy -előfizetésbe](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Erőforrások kezelése az Azure Portal használatával](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
