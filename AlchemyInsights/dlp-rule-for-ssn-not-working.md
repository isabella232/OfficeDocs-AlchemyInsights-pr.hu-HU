---
title: DLP szabály a TAJ-szám nem működik
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29474060"
---
<span data-ttu-id="1f184-p101">Hogy problémák adódnak az **Adatok elvesztésének megakadályozása (DLP)** tartalom a **Társadalombiztosítási szám (SSN)** tartalmazó, a bizalmas adatok típusa használatakor az Office 365 rendszerben nem működik? Ha igen, ellenőrizze, hogy a tartalom a DLP politika feladata a szükséges adatokat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="1f184-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="1f184-104">Például a TAJ-szám házirend konfigurálva 85 %-os megbízhatósági szint, a következő értékelik, és fel kell deríteni a kiváltó szabály:</span><span class="sxs-lookup"><span data-stu-id="1f184-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="1f184-105">**[Formátum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 számjegy, esetleg egy formázott vagy nem formázott minta</span><span class="sxs-lookup"><span data-stu-id="1f184-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="1f184-106">**[Minta:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** A négy különböző mintázatú SSNs négy függvény keresése:</span><span class="sxs-lookup"><span data-stu-id="1f184-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="1f184-107">Func_ssn SSNs pre-2011 erős formátummal formázott kötőjeleket és szóközöket (nnn-nn-nnnn vagy ddd nn dddd) talál.</span><span class="sxs-lookup"><span data-stu-id="1f184-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="1f184-108">Func_unformatted_ssn SSNs pre-2011 erős formázással, amelyek nem formázott, kilenc egymást követő számjegyből (ddddddddd) talál.</span><span class="sxs-lookup"><span data-stu-id="1f184-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="1f184-109">Func_randomized_formatted_ssn megtalálja a post-2011 SSNs formázott kötőjeleket és szóközöket (nnn-nn-nnnn vagy ddd nn dddd)</span><span class="sxs-lookup"><span data-stu-id="1f184-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="1f184-110">Func_randomized_unformatted_ssn megtalálja a post-2011 SSNs, amelyek nem formázott, kilenc egymást követő számjegyből (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="1f184-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="1f184-111">**[Ellenőrző összeg:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nem, nincs nincs ellenőrzőösszeg</span><span class="sxs-lookup"><span data-stu-id="1f184-111">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="1f184-112">**[Meghatározása:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP házirend abban, hogy ilyen jellegű érzékeny adatokat észlelt 85 % Ha belül a közelében 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="1f184-112">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="1f184-113">A [függvény Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) tartalom, amely megfelel a minta keresése.</span><span class="sxs-lookup"><span data-stu-id="1f184-113">The [function Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="1f184-p102">A [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) kulcsszó található. Példák a kulcsszavakat tartalmazza: *társadalombiztosítási, társadalombiztosítási #, Soc (mp), a TAJ-szám* . Például a TAJ-szám DLP házirend megjelenik a következő minta: **Taj-szám: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="1f184-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="1f184-117">Mi az SSNs a tartalom kimutatásához szükséges további tájékoztatást a következő részben a cikkben: [Mi az érzékeny adattípusok SSNs keresése](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="1f184-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="1f184-118">A beépített érzékeny információk különböző típusú cikke információ szükséges egyéb Újdonságok: [keressen Mi a bizalmas információk típusai](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="1f184-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

