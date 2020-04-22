---
title: DLP-szabály az amerikai bankszámlaszám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704041"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="87480-102">DLP-problémák az amerikai bankszámlaszámokkal</span><span class="sxs-lookup"><span data-stu-id="87480-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="87480-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="87480-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="87480-104">**DLP-problémák az amerikai bankszámlaszámokkal**</span><span class="sxs-lookup"><span data-stu-id="87480-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="87480-105">Problémái vannak az **adatveszteség-megelőzéssel (DLP),** amely nem működik **az amerikai bankszámlaszámot** tartalmazó tartalom esetében, amikor Az O365-ben DLP-érzékeny információtípust használ?</span><span class="sxs-lookup"><span data-stu-id="87480-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="87480-106">Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat, amit a DLP-házirend keres, amikor kiértékeli.</span><span class="sxs-lookup"><span data-stu-id="87480-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="87480-107">A 85%-os megbízhatósági szinttel konfigurált **US Bankszámlaszám-házirend** esetében például a rendszer a következőket értékeli ki, és a szabály aktiválásához észlelni kell:</span><span class="sxs-lookup"><span data-stu-id="87480-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="87480-108">**[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 számjegy</span><span class="sxs-lookup"><span data-stu-id="87480-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="87480-109">**[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 egymást követő számjegy.</span><span class="sxs-lookup"><span data-stu-id="87480-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="87480-110">**[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nem, nincs Checksum</span><span class="sxs-lookup"><span data-stu-id="87480-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="87480-111">**[Meghatározás:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP-házirend 75%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:</span><span class="sxs-lookup"><span data-stu-id="87480-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="87480-112">A reguláris kifejezés Regex_usa_bank_account_number a mintának megfelelő tartalmat talál</span><span class="sxs-lookup"><span data-stu-id="87480-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="87480-113">A Keyword_usa_Bank_Account kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="87480-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="87480-114">Például a következő minta aktiválódik az **Amerikai Egyesült Államok bankszámlaszám-házirendjének:** 78344011 folyószámla</span><span class="sxs-lookup"><span data-stu-id="87480-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="87480-115">Ha többet szeretne tudni arról, hogy mi szükséges ahhoz, hogy **egy amerikai bankszámlaszámot** észleljen a tartalomhoz, olvassa el a cikk következő szakaszát: [A bizalmas információtípusok az USA bankszámlaszámát keresik?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="87480-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="87480-116">Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="87480-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  