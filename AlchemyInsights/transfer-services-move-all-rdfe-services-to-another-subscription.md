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
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="26734-102">Átviteli szolgáltatások – az összes RDFE-szolgáltatás áthelyezése másik előfizetésbe</span><span class="sxs-lookup"><span data-stu-id="26734-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="26734-103">**Erőforrások áthelyezése**</span><span class="sxs-lookup"><span data-stu-id="26734-103">**Move resources**</span></span>

<span data-ttu-id="26734-104">Az Azure-erőforrásokat az Azure Portal, az Azure PowerShell, az Azure CLI vagy a REST API segítségével áthelyezheti egy másik Azure-előfizetésbe vagy erőforrás-csoportba az erőforrások áthelyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="26734-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="26734-105">Az erőforrások áthelyezése előtt az alábbiakra van lehetősége:</span><span class="sxs-lookup"><span data-stu-id="26734-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="26734-106">Ellenőrzőlista az erőforrások áthelyezése előtt</span><span class="sxs-lookup"><span data-stu-id="26734-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="26734-107">Áthelyezhető szolgáltatások</span><span class="sxs-lookup"><span data-stu-id="26734-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="26734-108">Az áthelyezés érvényesítése</span><span class="sxs-lookup"><span data-stu-id="26734-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="26734-109">Útmutatás áthelyezése a szolgáltatásokhoz</span><span class="sxs-lookup"><span data-stu-id="26734-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="26734-110">Ha a meglévő erőforrásokat át szeretné helyezni egy másik erőforráscsoporthoz vagy előfizetésbe, az alábbiakat használhatja:</span><span class="sxs-lookup"><span data-stu-id="26734-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="26734-111">Azure-portál</span><span class="sxs-lookup"><span data-stu-id="26734-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="26734-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="26734-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="26734-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="26734-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="26734-114">REST API</span><span class="sxs-lookup"><span data-stu-id="26734-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="26734-115">Oktatóanyag: [Az Azure-erőforrások áthelyezése másik erőforrás-csoportba vagy-előfizetésbe](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="26734-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="26734-116">**Az Azure Resource Manager hibáinak elhárítása**</span><span class="sxs-lookup"><span data-stu-id="26734-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="26734-117">Az alábbi cikkekből megtudhatja, hogy miként találhatja meg az Azure néhány gyakori központi telepítési hibáját, és hogyan kaphat információt a megoldásához.</span><span class="sxs-lookup"><span data-stu-id="26734-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="26734-118">Ha nem találja a központi telepítő hibájának megfelelő hibakódot, olvassa el a [hibakód keresése](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)című témakört.</span><span class="sxs-lookup"><span data-stu-id="26734-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="26734-119">A központi telepítő hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="26734-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="26734-120">Azure-erőforrások új erőforráscsoporthoz vagy előfizetésbe való áthelyezésével kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="26734-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="26734-121">Felhívjuk a figyelmét arra, hogy ha frissíteni szeretné az Azure-előfizetését, például az ingyenes fizetésről a befizetésre, az előfizetést konvertálnia kell.</span><span class="sxs-lookup"><span data-stu-id="26734-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="26734-122">Ha frissíteni szeretne egy ingyenes próbaverziót, olvassa el [az ingyenes próbaverzió frissítése vagy a Microsoft Imagine Azure-előfizetés a fizetéshez](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="26734-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="26734-123">Ha egy fizetési mód szerinti fizetési módot szeretné módosítani, olvassa el az [Azure Pay-as-your-go-előfizetés módosítása másik ajánlatra](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)című témakört.</span><span class="sxs-lookup"><span data-stu-id="26734-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="26734-124">**Azure-előfizetés hozzáadása vagy társítása az Azure Active Directory-bérlői webhelyhez:**</span><span class="sxs-lookup"><span data-stu-id="26734-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="26734-125">Bejelentkezés, és válassza ki a használni kívánt előfizetést az [Azure Portal előfizetések lapjáról](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="26734-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="26734-126">Válassza a **címtár módosítása** elemet.</span><span class="sxs-lookup"><span data-stu-id="26734-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="26734-127">Ellenőrizze a megjelenő figyelmeztetéseket, majd kattintson a **módosítás** gombra.</span><span class="sxs-lookup"><span data-stu-id="26734-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="26734-128">Az előfizetés megváltoztatja a címtárat, és sikerről szóló üzenetet kap.</span><span class="sxs-lookup"><span data-stu-id="26734-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="26734-129">Nyissa meg az új könyvtárat a *címtár* -kapcsoló használatával.</span><span class="sxs-lookup"><span data-stu-id="26734-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="26734-130">Akár 10 percet is igénybe vehet, hogy minden megfelelően megjelenjen.</span><span class="sxs-lookup"><span data-stu-id="26734-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="26734-131">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="26734-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="26734-132">Azure-előfizetés tulajdonjogának átvitele</span><span class="sxs-lookup"><span data-stu-id="26734-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="26734-133">Erőforrások áthelyezése új erőforrás-csoportba vagy előfizetésbe</span><span class="sxs-lookup"><span data-stu-id="26734-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="26734-134">Erőforrások kezelése az Azure Portal segítségével</span><span class="sxs-lookup"><span data-stu-id="26734-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
