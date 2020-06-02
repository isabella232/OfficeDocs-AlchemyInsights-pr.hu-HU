---
title: A DLP nem a várt módon működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507480"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e3594-102">A DLP nem a várt módon működik</span><span class="sxs-lookup"><span data-stu-id="e3594-102">DLP not working as expected</span></span>

<span data-ttu-id="e3594-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="e3594-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="e3594-104">**A DLP beállítása**</span><span class="sxs-lookup"><span data-stu-id="e3594-104">**Setting up DLP**</span></span>

<span data-ttu-id="e3594-105">Problémái vannak az **adatvesztés-megelőzéssel (DLP)** az Office 365-ben, hogy nem a várt módon működnek?</span><span class="sxs-lookup"><span data-stu-id="e3594-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e3594-106">Ha igen, győződjön meg arról, hogy a **DLP-házirend** megfelelően van beállítva, és hogy az adatok tartalmazzák, amit a **DLP-házirend** keres, amikor kiértékelik.</span><span class="sxs-lookup"><span data-stu-id="e3594-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="e3594-107">A DLP-házirendek lehetővé teszik a szervezeten belüli bizalmas adatok azonosítását és védelmét.</span><span class="sxs-lookup"><span data-stu-id="e3594-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e3594-108">A DLP-házirendek beállításához használja az [itt](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)található információkat.</span><span class="sxs-lookup"><span data-stu-id="e3594-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="e3594-109">**Mit keresnek a DLP-házirendek?**</span><span class="sxs-lookup"><span data-stu-id="e3594-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e3594-110">A biztonsági és megfelelőségi központok **beépített bizalmas információtípusainak** használatakor a DLP-házirendek az ilyen bizalmas típusok észlelésekor konkrét mintákat és elemeket keresnek.</span><span class="sxs-lookup"><span data-stu-id="e3594-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e3594-111">**Beépített bizalmas információtípusok**</span><span class="sxs-lookup"><span data-stu-id="e3594-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e3594-112">A beépített bizalmas típusokról és a DLP-házirend ről a Bizalmas típus észlelésekor a következő témakörben talál tájékoztatást: [A bizalmas információtípusok keresetttémaköre.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e3594-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="e3594-113">**Egyéni bizalmas információtípusok**</span><span class="sxs-lookup"><span data-stu-id="e3594-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e3594-114">Ha egyéni bizalmas információtípusokat próbál létrehozni, az alábbi cikkben megtudhatja, hogyan hozhat létre egyéni bizalmas [szöveget: Egyéni bizalmas információtípus létrehozása](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="e3594-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e3594-115">**DLP-házirend tesztelése**</span><span class="sxs-lookup"><span data-stu-id="e3594-115">**Test a DLP policy**</span></span>

<span data-ttu-id="e3594-116">Ha az adatokat beépített vagy egyéni bizalmas adatoktípussal szeretné tesztelni, használja a **Teszttípus** beállítást a **Besorolások**  >  **bizalmas információtípusai**csoportban.</span><span class="sxs-lookup"><span data-stu-id="e3594-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e3594-117">További információt az [Egyéni bizalmas információtípusok tesztelése](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="e3594-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e3594-118">**Jelentések**</span><span class="sxs-lookup"><span data-stu-id="e3594-118">**Reports**</span></span>
  
- <span data-ttu-id="e3594-119">Bizalmas adatok betekintést nyerhet a [DLP-jelentések segítségével.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="e3594-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e3594-120">Az esemény konkrét részleteinek megtekintése [incidensjelentéssel.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="e3594-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
