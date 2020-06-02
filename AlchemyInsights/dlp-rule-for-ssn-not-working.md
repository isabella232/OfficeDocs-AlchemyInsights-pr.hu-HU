---
title: DLP-szabály nem működik az SSN-hez
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507372"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="ae990-102">DLP kérdések társadalombiztosítási számok</span><span class="sxs-lookup"><span data-stu-id="ae990-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="ae990-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="ae990-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ae990-104">**DLP-problémák az SSN-ekkel**</span><span class="sxs-lookup"><span data-stu-id="ae990-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="ae990-105">Problémái vannak azzal, hogy **a** Microsoft 365-ben bizalmas információtípushasználata esetén nem működik a **társadalombiztosítási számot (SSN)** tartalmazó tartalom használata?</span><span class="sxs-lookup"><span data-stu-id="ae990-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="ae990-106">Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat, amit a DLP-házirend keres.</span><span class="sxs-lookup"><span data-stu-id="ae990-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="ae990-107">Például egy 85%-os megbízhatósági szinttel konfigurált SSN-házirend esetén a rendszer a következőket értékeli ki, és a szabály aktiválásához észlelni kell:</span><span class="sxs-lookup"><span data-stu-id="ae990-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="ae990-108">**[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 számjegy, amely formázott vagy formázatlan minta lehet</span><span class="sxs-lookup"><span data-stu-id="ae990-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="ae990-109">**[Minta:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Négy függvény négy különböző mintában keres SSN-eket:</span><span class="sxs-lookup"><span data-stu-id="ae990-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="ae990-110">Func_ssn a 2011 előtti erős formázású SSN-eket szaggatott vagy szóközzel formázott (ddd-dd-ddd VAGY ddd dddd) formázott ssn-eket keres.</span><span class="sxs-lookup"><span data-stu-id="ae990-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="ae990-111">Func_unformatted_ssn a 2011 előtti erős formázású SSN-eket kilenc egymást követő számjegyként (dddddddd) formázza.</span><span class="sxs-lookup"><span data-stu-id="ae990-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="ae990-112">Func_randomized_formatted_ssn 2011 utáni, kötőjelekkel vagy szóközökkel formázott SSN-eket keres (ddd-dd-ddd VAGY ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="ae990-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="ae990-113">Func_randomized_unformatted_ssn a 2011 utáni SSN-eket kilenc egymást követő számjegyként formázva találja meg (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="ae990-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="ae990-114">**[Ellenőrző összeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nem, nincs Checksum</span><span class="sxs-lookup"><span data-stu-id="ae990-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="ae990-115">**[Meghatározás:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP-házirend 85%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:</span><span class="sxs-lookup"><span data-stu-id="ae990-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ae990-116">A [Func_ssn függvény](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) a mintának megfelelő tartalmat talál.</span><span class="sxs-lookup"><span data-stu-id="ae990-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ae990-117">A [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="ae990-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="ae990-118">Példák a kulcsszavak közé tartozik: *Társadalombiztosítási, Társadalombiztosítási #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="ae990-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="ae990-119">Például a következő minta aktiválódik a DLP SSN-házirend: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="ae990-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="ae990-120">Ha többet szeretne tudni arról, hogy mi szükséges az SSN-ek észleléséhez a tartalomhoz, olvassa el a cikk következő szakaszát: [A bizalmas információtípusok mit keresnek az SSN-ek számára?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="ae990-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="ae990-121">Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="ae990-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  