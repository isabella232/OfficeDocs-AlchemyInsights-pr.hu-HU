---
title: AIP-címkés házirendek létrehozása
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569203"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="4e256-102">AIP-címkés házirendek létrehozása</span><span class="sxs-lookup"><span data-stu-id="4e256-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="4e256-103">Az Azure Information Protection(AIP) címkék a szervezet által általában létrehozott és a személyes adatok legalacsonyabb besorolásától a rendkívül bizalmas adatok legmagasabb besorolásától kezdve az adatok teljes körével használhatók.</span><span class="sxs-lookup"><span data-stu-id="4e256-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="4e256-104">Az Azure Information Protection Szabályzatok az Azure Information Protection (AIP) klasszikus ügyfélre vonatkoznak, nem pedig az [AIP unified labeling ügyfélre.](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)</span><span class="sxs-lookup"><span data-stu-id="4e256-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="4e256-105">Az AIP-házirendben több elemet is konfigurálhat, például a következő lehetőségeket:</span><span class="sxs-lookup"><span data-stu-id="4e256-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="4e256-106">Lehetőség, amely címke lehetővé teszi a rendszergazdák vagy a felhasználó osztályozza és védelem (választható) dokumentumok és e-mailek</span><span class="sxs-lookup"><span data-stu-id="4e256-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="4e256-107">A besorolás kényszerítése dokumentumok mentésekor és e-mailek küldésekor</span><span class="sxs-lookup"><span data-stu-id="4e256-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="4e256-108">Lehetőség az e-mailek automatikus címkézésére a mellékletek alapján.</span><span class="sxs-lookup"><span data-stu-id="4e256-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="4e256-109">Annak szabályozására, hogy az Információvédelmi sáv megjelenjen-e az Office-alkalmazásokban</span><span class="sxs-lookup"><span data-stu-id="4e256-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="4e256-110">Az Azure Information Protection szabályzatokkal kapcsolatos további lehetőségeket és információkat a következő [témakörben találja: Az Azure Information Protection szabályzat áttekintése.](https://docs.microsoft.com/azure/information-protection/overview-policy)</span><span class="sxs-lookup"><span data-stu-id="4e256-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="4e256-111">Az AIP-házirendekkel kapcsolatos egyéb hasznos forrásoka következő témakörben jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="4e256-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="4e256-112">Oktatóanyag: Konfigurálja az Azure Information Protection házirend-beállításait, és hozzon létre egy új címkét</span><span class="sxs-lookup"><span data-stu-id="4e256-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="4e256-113">Az Azure Information Protection szabályzat konfigurálása</span><span class="sxs-lookup"><span data-stu-id="4e256-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="4e256-114">Érzékenységi címkék és házirendjeik létrehozása és konfigurálása</span><span class="sxs-lookup"><span data-stu-id="4e256-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="4e256-115">Útmutató útmutatók az Azure Information Protectiont használó gyakori forgatókönyvekhez</span><span class="sxs-lookup"><span data-stu-id="4e256-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="4e256-116">Tekintse át az Azure Information Protection dokumentációját</span><span class="sxs-lookup"><span data-stu-id="4e256-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="4e256-117">Az Azure-információvédelem követelményei</span><span class="sxs-lookup"><span data-stu-id="4e256-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="4e256-118">Rövid útmutató az Azure Information Protection szolgáltatáshoz</span><span class="sxs-lookup"><span data-stu-id="4e256-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="4e256-119">Az Azure Information Protection ügyfél letöltése</span><span class="sxs-lookup"><span data-stu-id="4e256-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)