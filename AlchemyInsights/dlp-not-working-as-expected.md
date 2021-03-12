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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707812"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="17577-102">A DLP nem a várt módon működik</span><span class="sxs-lookup"><span data-stu-id="17577-102">DLP not working as expected</span></span>

<span data-ttu-id="17577-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="17577-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="17577-104">**A DLP beállítása**</span><span class="sxs-lookup"><span data-stu-id="17577-104">**Setting up DLP**</span></span>

<span data-ttu-id="17577-105">Az Office 365 **adatveszteség-megelőzési (DLP)** problémái nem a várt módon működnek?</span><span class="sxs-lookup"><span data-stu-id="17577-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="17577-106">Ha igen, győződjön meg arról, hogy a **DLP-házirend** megfelelően van beállítva, és hogy az adatok azt tartalmazják, amit a **DLP-házirend** a kiértékeléskor keres.</span><span class="sxs-lookup"><span data-stu-id="17577-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="17577-107">A DLP-házirendek lehetővé teszik a bizalmas adatok azonosítását és védelmét a szervezetben.</span><span class="sxs-lookup"><span data-stu-id="17577-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="17577-108">A DLP-házirendek beállításához használja az itt [található információkat.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="17577-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="17577-109">**Milyen DLP-házirendeket keresnek?**</span><span class="sxs-lookup"><span data-stu-id="17577-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="17577-110">Amikor a biztonsági és megfelelőségi központok beépített bizalmas adattípusokat használ, a **DLP-házirendek** meghatározott mintákat és elemeket keresnek a bizalmas típusok észlelése során.</span><span class="sxs-lookup"><span data-stu-id="17577-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="17577-111">**Beépített bizalmas információtípusok**</span><span class="sxs-lookup"><span data-stu-id="17577-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="17577-112">A bizalmas típusú adatok beépített típusairól és arról, hogy a DLP-házirend mit keres a Bizalmas típus észlelése esetén: A bizalmas [adattípusok által kereshető információk.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="17577-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="17577-113">**Egyéni bizalmas információtípusok**</span><span class="sxs-lookup"><span data-stu-id="17577-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="17577-114">Ha egyéni bizalmas adattípusokat próbál létrehozni, az alábbi cikkben további információt talál az egyéni bizalmas adattípusok létrehozásáról: Egyéni bizalmas adattípus [létrehozása.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="17577-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="17577-115">**DLP-házirend tesztelése**</span><span class="sxs-lookup"><span data-stu-id="17577-115">**Test a DLP policy**</span></span>

<span data-ttu-id="17577-116">Ha egy beépített vagy egyéni bizalmasadat-típussal tesztelni kívánt adatokat, használja a Bizalmas adatok besorolása csoport Teszttípus   >  **beállítását.**</span><span class="sxs-lookup"><span data-stu-id="17577-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="17577-117">További információt az egyéni bizalmas [adattípusok tesztelése.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="17577-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="17577-118">**Jelentések**</span><span class="sxs-lookup"><span data-stu-id="17577-118">**Reports**</span></span>
  
- <span data-ttu-id="17577-119">Bizalmas adatelemzéseket kaphat a [DLP-jelentésekkel.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="17577-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="17577-120">Az esemény részleteinek megtekintése [incidensjelentéssel.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="17577-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
