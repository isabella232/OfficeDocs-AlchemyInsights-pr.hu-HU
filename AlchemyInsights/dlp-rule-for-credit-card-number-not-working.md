---
title: DLP-szabály a hitelkártyaszám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932445"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="5a468-102">DLP-problémák hitelkártyaszámokkal</span><span class="sxs-lookup"><span data-stu-id="5a468-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="5a468-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="5a468-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5a468-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="5a468-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5a468-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="5a468-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5a468-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="5a468-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5a468-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="5a468-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5a468-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="5a468-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5a468-109">**DLP-problémák hitelkártyaszámokkal**</span><span class="sxs-lookup"><span data-stu-id="5a468-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="5a468-110">Problémái vannak azzal, hogy **az Adatveszteség-megelőzés (DLP)** nem működik a **hitelkártyaszámot** tartalmazó tartalom esetében, amikor Az O365-ben DLP-érzékeny információtípust használ?</span><span class="sxs-lookup"><span data-stu-id="5a468-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="5a468-111">Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat a DLP-házirend aktiválásához a kiértékeléskor.</span><span class="sxs-lookup"><span data-stu-id="5a468-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="5a468-112">A 85%-os megbízhatósági szinttel konfigurált **hitelkártya-házirendek** esetében például a rendszer a következőket értékeli ki, és a szabály aktiválásához észlelni kell őket:</span><span class="sxs-lookup"><span data-stu-id="5a468-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="5a468-113">**[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 számjegy, amely formázható vagy formázható (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="5a468-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="5a468-114">**[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Nagyon összetett és robusztus minta, amely észleli a világ összes jelentős márkájának kártyáit, beleértve a Visa, MasterCard, Discover Card, JCB, American Express, ajándékkártyákat és étkezőkártyákat.</span><span class="sxs-lookup"><span data-stu-id="5a468-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="5a468-115">**[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Igen, a Luhn ellenőrző összeg</span><span class="sxs-lookup"><span data-stu-id="5a468-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="5a468-116">**[Meghatározás:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP-házirend 85%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:</span><span class="sxs-lookup"><span data-stu-id="5a468-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="5a468-117">A Func_credit_card függvény a mintának megfelelő tartalmat talál.</span><span class="sxs-lookup"><span data-stu-id="5a468-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="5a468-118">Az alábbiak egyike igaz:</span><span class="sxs-lookup"><span data-stu-id="5a468-118">One of the following is true:</span></span>

  - <span data-ttu-id="5a468-119">A Keyword_cc_verification kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="5a468-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="5a468-120">A Keyword_cc_name kulcsszó található</span><span class="sxs-lookup"><span data-stu-id="5a468-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="5a468-121">A Func_expiration_date függvény a megfelelő dátumformátumban keresi a dátumot.</span><span class="sxs-lookup"><span data-stu-id="5a468-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="5a468-122">Az ellenőrző összeg átmegy</span><span class="sxs-lookup"><span data-stu-id="5a468-122">The checksum passes</span></span>

    <span data-ttu-id="5a468-123">Például a következő minta a DLP hitelkártyaszám-házirendjének aktiválásához lépki:</span><span class="sxs-lookup"><span data-stu-id="5a468-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="5a468-124">Vízum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="5a468-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="5a468-125">Lejár: 2/2009</span><span class="sxs-lookup"><span data-stu-id="5a468-125">Expires: 2/2009</span></span>

<span data-ttu-id="5a468-126">Ha többet szeretne tudni arról, hogy mi szükséges a **hitelkártyaszám** észleléséhez a tartalomhoz, olvassa el a cikk következő szakaszát: [Milyen bizalmas információtípusok keresnek hitelkártyát#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="5a468-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="5a468-127">Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="5a468-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  