---
title: DLP szabály a TAJ-szám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389435"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="d0f5a-102">Társadalombiztosítási számok DLP problémái</span><span class="sxs-lookup"><span data-stu-id="d0f5a-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="d0f5a-103">Hogy problémák adódnak az **Adatok elvesztésének megakadályozása (DLP)** tartalom a **Társadalombiztosítási szám (SSN)** tartalmazó, a bizalmas adatok típusa használatakor az Office 365 rendszerben nem működik?</span><span class="sxs-lookup"><span data-stu-id="d0f5a-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="d0f5a-104">Ha igen, ellenőrizze, hogy a tartalom a DLP politika feladata a szükséges adatokat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="d0f5a-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="d0f5a-105">Például a TAJ-szám házirend konfigurálva 85 %-os megbízhatósági szint, a következő értékelik, és fel kell deríteni a kiváltó szabály:</span><span class="sxs-lookup"><span data-stu-id="d0f5a-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d0f5a-106">**[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 számjegy, esetleg egy formázott vagy nem formázott minta</span><span class="sxs-lookup"><span data-stu-id="d0f5a-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="d0f5a-107">**[Minta:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** A négy különböző mintázatú SSNs négy függvény keresése:</span><span class="sxs-lookup"><span data-stu-id="d0f5a-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="d0f5a-108">Func_ssn SSNs pre-2011 erős formátummal formázott kötőjeleket és szóközöket (nnn-nn-nnnn vagy ddd nn dddd) talál.</span><span class="sxs-lookup"><span data-stu-id="d0f5a-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d0f5a-109">Func_unformatted_ssn SSNs pre-2011 erős formázással, amelyek nem formázott, kilenc egymást követő számjegyből (ddddddddd) talál.</span><span class="sxs-lookup"><span data-stu-id="d0f5a-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="d0f5a-110">Func_randomized_formatted_ssn megtalálja a post-2011 SSNs formázott kötőjeleket és szóközöket (nnn-nn-nnnn vagy ddd nn dddd)</span><span class="sxs-lookup"><span data-stu-id="d0f5a-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d0f5a-111">Func_randomized_unformatted_ssn megtalálja a post-2011 SSNs, amelyek nem formázott, kilenc egymást követő számjegyből (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="d0f5a-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="d0f5a-112">**[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nem, nincs nincs ellenőrzőösszeg</span><span class="sxs-lookup"><span data-stu-id="d0f5a-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="d0f5a-113">**[Meghatározása:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP házirend abban, hogy ilyen jellegű érzékeny adatokat észlelt 85 % Ha belül a közelében 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="d0f5a-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d0f5a-114">A [függvény Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) tartalom, amely megfelel a minta keresése.</span><span class="sxs-lookup"><span data-stu-id="d0f5a-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d0f5a-115">A [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="d0f5a-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="d0f5a-116">Példák a kulcsszavakat tartalmazza: *társadalombiztosítási, társadalombiztosítási #, Soc (mp), a TAJ-szám* .</span><span class="sxs-lookup"><span data-stu-id="d0f5a-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="d0f5a-117">Például a TAJ-szám DLP házirend megjelenik a következő minta: **Taj-szám: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="d0f5a-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="d0f5a-118">Mi az SSNs a tartalom kimutatásához szükséges további tájékoztatást a következő részben a cikkben: [Mi az érzékeny adattípusok SSNs keresése](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="d0f5a-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="d0f5a-119">A beépített érzékeny információk különböző típusú cikke információ szükséges egyéb Újdonságok: [keressen Mi a bizalmas információk típusai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d0f5a-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  