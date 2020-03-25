---
title: DLP-szabály nem működik az SSN-hez
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
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932525"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="4861a-102">DLP kérdések társadalombiztosítási számok</span><span class="sxs-lookup"><span data-stu-id="4861a-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="4861a-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="4861a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4861a-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="4861a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4861a-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="4861a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4861a-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="4861a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4861a-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="4861a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4861a-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="4861a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4861a-109">**DLP-problémák az SSN-ekkel**</span><span class="sxs-lookup"><span data-stu-id="4861a-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="4861a-110">Problémái vannak azzal, hogy **az Adatvesztés-megelőzés (DLP)** nem működik a **társadalombiztosítási számot (SSN)** tartalmazó tartalom esetében, amikor bizalmas információtípust használ az Office 365-ben?</span><span class="sxs-lookup"><span data-stu-id="4861a-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="4861a-111">Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat, amit a DLP-házirend keres.</span><span class="sxs-lookup"><span data-stu-id="4861a-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4861a-112">Például egy 85%-os megbízhatósági szinttel konfigurált SSN-házirend esetén a rendszer a következőket értékeli ki, és a szabály aktiválásához észlelni kell:</span><span class="sxs-lookup"><span data-stu-id="4861a-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4861a-113">**[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 számjegy, amely formázott vagy formázatlan minta lehet</span><span class="sxs-lookup"><span data-stu-id="4861a-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="4861a-114">**[Minta:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Négy függvény négy különböző mintában keres SSN-eket:</span><span class="sxs-lookup"><span data-stu-id="4861a-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="4861a-115">Func_ssn a 2011 előtti erős formázású SSN-eket szaggatott vagy szóközzel formázott (ddd-dd-ddd VAGY ddd dddd) formázott ssn-eket keres.</span><span class="sxs-lookup"><span data-stu-id="4861a-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4861a-116">Func_unformatted_ssn a 2011 előtti erős formázású SSN-eket kilenc egymást követő számjegyként (dddddddd) formázza.</span><span class="sxs-lookup"><span data-stu-id="4861a-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="4861a-117">Func_randomized_formatted_ssn 2011 utáni, kötőjelekkel vagy szóközökkel formázott SSN-eket keres (ddd-dd-ddd VAGY ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="4861a-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4861a-118">Func_randomized_unformatted_ssn a 2011 utáni SSN-eket kilenc egymást követő számjegyként formázva találja meg (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="4861a-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="4861a-119">**[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nem, nincs Checksum</span><span class="sxs-lookup"><span data-stu-id="4861a-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="4861a-120">**[Meghatározás:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP-házirend 85%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:</span><span class="sxs-lookup"><span data-stu-id="4861a-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4861a-121">A [Func_ssn függvény](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) a mintának megfelelő tartalmat talál.</span><span class="sxs-lookup"><span data-stu-id="4861a-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4861a-122">A [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="4861a-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="4861a-123">Példák a kulcsszavak közé tartozik: *Társadalombiztosítási, Társadalombiztosítási #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="4861a-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="4861a-124">Például a következő minta aktiválódik a DLP SSN-házirend: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="4861a-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="4861a-125">Ha többet szeretne tudni arról, hogy mi szükséges az SSN-ek észleléséhez a tartalomhoz, olvassa el a cikk következő szakaszát: [A bizalmas információtípusok mit keresnek az SSN-ek számára?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="4861a-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4861a-126">Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="4861a-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  