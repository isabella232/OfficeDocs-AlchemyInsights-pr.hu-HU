---
title: DLP nem a várt módon működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941070"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="f2965-102">DLP nem a várt módon működik</span><span class="sxs-lookup"><span data-stu-id="f2965-102">DLP not working as expected</span></span>

<span data-ttu-id="f2965-103">Hogy problémák adódnak az **Adatok elvesztésének megakadályozása (DLP)** az Office 365 rendszerben nem a várt módon működik?</span><span class="sxs-lookup"><span data-stu-id="f2965-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="f2965-104">Ha igen, ellenőrizze a **DLP házirend** helyesen van beállítva, és, hogy az adatok milyen a **DLP házirendet** tartalmaz keres Ha értékelt van.</span><span class="sxs-lookup"><span data-stu-id="f2965-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="f2965-105">**DLP beállítása**</span><span class="sxs-lookup"><span data-stu-id="f2965-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="f2965-106">DLP házirendek segítségével azonosítása és a szervezet bizalmas információk védelme.</span><span class="sxs-lookup"><span data-stu-id="f2965-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="f2965-107">DLP irányelvek beállítása, az információk [Itt](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="f2965-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="f2965-108">**Milyen DLP házirendek keresése**</span><span class="sxs-lookup"><span data-stu-id="f2965-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="f2965-109">Ha a **bizalmas adatok beépített típusok** használata az Office 365 biztonsági és kompatibilitási központ, DLP házirendek keresni bizonyos minták és elemek érzékeny típusaival észlelése esetén.</span><span class="sxs-lookup"><span data-stu-id="f2965-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="f2965-110">**Bizalmas adatok beépített típusok**</span><span class="sxs-lookup"><span data-stu-id="f2965-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="f2965-111">A beépített érzékeny típusok és mi DLP házirendet keres az érzékeny típus észlelése esetén információt: [a bizalmas adatok milyen keresni](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="f2965-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="f2965-112">**Egyéni bizalmas adatok típusai**</span><span class="sxs-lookup"><span data-stu-id="f2965-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="f2965-113">Próbál létrehozni egyéni bizalmas adatokat, ha használja a következő cikkben olvashat arról, hogyan hozhat létre egyéni érzékeny típusok: [létrehozása a egyéni bizalmas adatok típusa](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="f2965-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="f2965-114">**A DLP házirend tesztelése**</span><span class="sxs-lookup"><span data-stu-id="f2965-114">**Test a DLP policy**</span></span>

<span data-ttu-id="f2965-115">Ellenőrizheti az adatokat, és a beépített vagy egyéni bizalmas adatok típusa, használja a **Teszttípus** lehetőség szerinti **osztályozás** > **bizalmas információ típusát**.</span><span class="sxs-lookup"><span data-stu-id="f2965-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="f2965-116">További információért lásd a [Teszttípus egyéni bizalmas adatokat](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="f2965-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="f2965-117">**Jelentések**</span><span class="sxs-lookup"><span data-stu-id="f2965-117">**Reports**</span></span>
  
- <span data-ttu-id="f2965-118">A bizalmas adatok elképzelések Get [DLP jelentések.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="f2965-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="f2965-119">Lásd a részleteket az esemény, [Baleset-jelentés](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="f2965-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
