---
title: DLP szabály az USA/Uk útlevélszám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977108"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="49173-102">Problémák a DLP - USA / Uk útlevél számok</span><span class="sxs-lookup"><span data-stu-id="49173-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="49173-103">**Fontos:** Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is magas rendelkezésre állásúak maradjanak – további információkért látogasson el a [SharePoint Online ideiglenes szolgáltatásának korrekcióira.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="49173-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="49173-104">**DLP kérdések az USA/Egyesült Királyság útlevélszámokkal**</span><span class="sxs-lookup"><span data-stu-id="49173-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="49173-105">Problémái vannak az **adatveszteség-megelőzéssel (DLP),** amely nem működik **az egyesült államokbeli/egyesült királyságbeli útlevélszámot** tartalmazó tartalom esetében, amikor Az O365-ben DLP-érzékeny információtípust használ?</span><span class="sxs-lookup"><span data-stu-id="49173-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="49173-106">Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat, amit a DLP-házirend keres, amikor kiértékeli.</span><span class="sxs-lookup"><span data-stu-id="49173-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="49173-107">Például egy 75%-os megbízhatósági szinttel konfigurált **egyesült államokbeli/brit útlevélszám-házirend** esetében a rendszer kiértékeli a következőket, és a szabály aktiválásához észlelni kell őket.</span><span class="sxs-lookup"><span data-stu-id="49173-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="49173-108">**[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Kilenc számjegy</span><span class="sxs-lookup"><span data-stu-id="49173-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="49173-109">**[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Kilenc egymást követő számjegy</span><span class="sxs-lookup"><span data-stu-id="49173-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="49173-110">**[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nem, nincs Checksum</span><span class="sxs-lookup"><span data-stu-id="49173-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="49173-111">**[Meghatározás:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP-házirend 75%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:</span><span class="sxs-lookup"><span data-stu-id="49173-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="49173-112">A Func_usa_uk_passport függvény a mintának megfelelő tartalmat talál.</span><span class="sxs-lookup"><span data-stu-id="49173-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="49173-113">A Keyword_passport kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="49173-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="49173-114">Például a következő minta váltaná ki az **Egyesült Államok/Egyesült Királyság útlevélszámra** vonatkozó politikáját: U.S. Passport number 123456789</span><span class="sxs-lookup"><span data-stu-id="49173-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="49173-115">Ha többet szeretne tudni arról, hogy mi szükséges az Egyesült Államok/Egyesült Királyság útlevélszám észleléséhez a tartalomhoz, olvassa el a cikk következő szakaszát: [A bizalmas információtípusok az USA/UK útlevélszámát keresik?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="49173-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="49173-116">Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="49173-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  