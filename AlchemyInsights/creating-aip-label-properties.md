---
title: Az adattervezési címke házirendjeinek létrehozása
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732177"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="88c1e-102">Az adattervezési címke házirendjeinek létrehozása</span><span class="sxs-lookup"><span data-stu-id="88c1e-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="88c1e-103">Az Azure Information Protection (Active Information Protection) címkéi a teljes adattartományban használhatók, amelyeket egy szervezet általában a személyes adatok legalacsonyabb besorolásával hoz létre és tárol a nagyon bizalmas adatok legmagasabb besorolásához.</span><span class="sxs-lookup"><span data-stu-id="88c1e-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="88c1e-104">Az Azure Information Protection házirendek az Azure Information Protection ("" Information Protection ("" ") klasszikus ügyfélprogramot, és  [nem az"](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)e</span><span class="sxs-lookup"><span data-stu-id="88c1e-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="88c1e-105">A rendszergazda-házirendben több elemet is beállíthat, például az alábbi beállításokat:</span><span class="sxs-lookup"><span data-stu-id="88c1e-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="88c1e-106">Az a beállítás, amelyhez a címke tájékoztatja a rendszergazdákat vagy a felhasználók osztályozását és védelmét (nem kötelező) a dokumentumokat és e-maileket.</span><span class="sxs-lookup"><span data-stu-id="88c1e-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="88c1e-107">Az osztályozás kényszerítése a dokumentumok mentésekor és e-mailek küldésekor</span><span class="sxs-lookup"><span data-stu-id="88c1e-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="88c1e-108">Az e-mailek automatikus címkézésének lehetősége a mellékletek alapján.</span><span class="sxs-lookup"><span data-stu-id="88c1e-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="88c1e-109">Annak szabályozása, hogy az adatvédelemi sáv megjelenjen-e az Office-alkalmazásokban</span><span class="sxs-lookup"><span data-stu-id="88c1e-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="88c1e-110">Az Azure Information Protection Policy szolgáltatással kapcsolatos további lehetőségekről további információt a következő témakörben talál: [Az Azure Information Protection Policy áttekintése](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="88c1e-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="88c1e-111">További hasznos források az alábbi cikkekben:</span><span class="sxs-lookup"><span data-stu-id="88c1e-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="88c1e-112">Oktatóanyag: az Azure Information Protection Policy beállításainak megadása és új címke létrehozása</span><span class="sxs-lookup"><span data-stu-id="88c1e-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="88c1e-113">Az Azure Information Protection Policy konfigurálása</span><span class="sxs-lookup"><span data-stu-id="88c1e-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="88c1e-114">Tartalmi címkék és a hozzájuk tartozó házirendek létrehozása és beállítása</span><span class="sxs-lookup"><span data-stu-id="88c1e-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="88c1e-115">Útmutatók az Azure-adatvédelemt használó gyakori forgatókönyvekhez</span><span class="sxs-lookup"><span data-stu-id="88c1e-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="88c1e-116">Az Azure Information Protection dokumentációjának áttekintése</span><span class="sxs-lookup"><span data-stu-id="88c1e-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="88c1e-117">Az Azure Information Protection követelményei</span><span class="sxs-lookup"><span data-stu-id="88c1e-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="88c1e-118">Rövid útmutató az Azure Information Protectionhez</span><span class="sxs-lookup"><span data-stu-id="88c1e-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="88c1e-119">Az Azure Information Protection ügyfélprogram letöltése</span><span class="sxs-lookup"><span data-stu-id="88c1e-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)