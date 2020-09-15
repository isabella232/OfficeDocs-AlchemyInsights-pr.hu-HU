---
title: A DLP nem a várt módon működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679695"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="52098-102">A DLP nem a várt módon működik</span><span class="sxs-lookup"><span data-stu-id="52098-102">DLP not working as expected</span></span>

<span data-ttu-id="52098-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="52098-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="52098-104">**DLP beállítása**</span><span class="sxs-lookup"><span data-stu-id="52098-104">**Setting up DLP**</span></span>

<span data-ttu-id="52098-105">Problémát tapasztal az **adatvesztés-megelőzés (DLP)** használatakor az Office 365-ben, nem a várt módon működik?</span><span class="sxs-lookup"><span data-stu-id="52098-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="52098-106">Ha igen, győződjön meg arról, hogy a **DLP-házirend** megfelelően van beállítva, és hogy az Ön által kiértékeléskor az Ön által használt **DLP-házirend** milyen információkat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="52098-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="52098-107">A DLP-házirendekkel bizalmas információkat azonosíthat és védheti meg a szervezetében.</span><span class="sxs-lookup"><span data-stu-id="52098-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="52098-108">A DLP-házirendek beállításához használja az [alábbi](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)információkat.</span><span class="sxs-lookup"><span data-stu-id="52098-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="52098-109">**Milyen DLP-házirendeket keres**</span><span class="sxs-lookup"><span data-stu-id="52098-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="52098-110">A biztonsági és megfelelőségi központokban a **beépített bizalmas adattípusok** használatakor a DLP-házirendek bizonyos mintázatokat és elemeket keresnek a bizalmas típusok észlelése során.</span><span class="sxs-lookup"><span data-stu-id="52098-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="52098-111">**Beépített bizalmas adattípusok**</span><span class="sxs-lookup"><span data-stu-id="52098-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="52098-112">A beépített bizalmas típusokról, valamint arról, hogy milyen típusú DLP-házirendet keres a bizalmas típus észlelése során, a következő témakörben talál információt: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="52098-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="52098-113">**Egyéni bizalmas adattípusok**</span><span class="sxs-lookup"><span data-stu-id="52098-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="52098-114">Ha egyéni bizalmas adattípusokat próbál létrehozni, az alábbi cikkből megtudhatja, hogy miként hozhat létre egyéni bizalmas típust: [Egyéni bizalmas adattípus létrehozása](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="52098-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="52098-115">**DLP-házirend tesztelése**</span><span class="sxs-lookup"><span data-stu-id="52098-115">**Test a DLP policy**</span></span>

<span data-ttu-id="52098-116">Ha egy beépített vagy egyéni bizalmas adattípussal szeretné tesztelni az adatokat, használja a **típus típusa** beállítást a bizalmas adatok **osztályozása**csoportban  >  **Sensitive info types**.</span><span class="sxs-lookup"><span data-stu-id="52098-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="52098-117">További információt az [Egyéni bizalmas adattípusok tesztelése](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="52098-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="52098-118">**Jelentések**</span><span class="sxs-lookup"><span data-stu-id="52098-118">**Reports**</span></span>
  
- <span data-ttu-id="52098-119">Az adatok bizalmasan jelennek meg [DLP-jelentésekkel.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="52098-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="52098-120">Az esemény konkrét részleteinek megtekintése incidens- [jelentéssel](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="52098-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
