---
title: DLP szabály nem működik a hitelkártya száma
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
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389579"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="e3f17-102">DLP problémáinak hitelkártyaszámok</span><span class="sxs-lookup"><span data-stu-id="e3f17-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="e3f17-103">Az **Adatok elvesztésének megakadályozása (DLP)** nem működik a tartalom egy **Hitelkártya számát** tartalmazó, O365 a DLP érzékeny adatok típusa használatakor problémák lépnek?</span><span class="sxs-lookup"><span data-stu-id="e3f17-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e3f17-104">Ha igen, ellenőrizze, hogy a tartalom tartalmazza az aktiváláshoz szükséges adatokat az a DLP házirendet, amikor azt értékelik.</span><span class="sxs-lookup"><span data-stu-id="e3f17-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="e3f17-105">Például **hitelkártya-házirend** konfigurálva 85 %-os megbízhatósági szint, a következő értékelik, és fel kell deríteni a kiváltó szabály:</span><span class="sxs-lookup"><span data-stu-id="e3f17-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="e3f17-106">**[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 számjegyből állhatnak, amelyek formázhatók vagy formázatlan (dddddddddddddddd), és meg kell felelnie a Luhn.</span><span class="sxs-lookup"><span data-stu-id="e3f17-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="e3f17-107">**[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Nagyon bonyolult és nagy teljesítményű minta által észlelt minden jelentős márka világszerte, beleértve a Visa, MasterCard, Fedezze fel a kártya, JCB, American Express, ajándékutalványok és diner kártyák kártyáit.</span><span class="sxs-lookup"><span data-stu-id="e3f17-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="e3f17-108">**[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Igen, a Luhn-ellenőrzőösszeg</span><span class="sxs-lookup"><span data-stu-id="e3f17-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="e3f17-109">**[Meghatározása:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP házirend abban, hogy ilyen jellegű érzékeny adatokat észlelt 85 % Ha belül a közelében 300 karakter:</span><span class="sxs-lookup"><span data-stu-id="e3f17-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e3f17-110">A függvény Func_credit_card tartalom, amely megfelel a minta keresése.</span><span class="sxs-lookup"><span data-stu-id="e3f17-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="e3f17-111">A következők egyike igaz:</span><span class="sxs-lookup"><span data-stu-id="e3f17-111">One of the following is true:</span></span>

  - <span data-ttu-id="e3f17-112">A Keyword_cc_verification kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="e3f17-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="e3f17-113">A Keyword_cc_name kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="e3f17-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="e3f17-114">A Func_expiration_date függvény dátum megkeresi a megfelelő dátum formátuma.</span><span class="sxs-lookup"><span data-stu-id="e3f17-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="e3f17-115">Az ellenőrzőösszeg fázisok</span><span class="sxs-lookup"><span data-stu-id="e3f17-115">The checksum passes</span></span>

    <span data-ttu-id="e3f17-116">Például a következő minta DLP hitelkártya száma házirend megjelenik:</span><span class="sxs-lookup"><span data-stu-id="e3f17-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="e3f17-117">Vízum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="e3f17-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="e3f17-118">Lejár: 2/2009</span><span class="sxs-lookup"><span data-stu-id="e3f17-118">Expires: 2/2009</span></span>

<span data-ttu-id="e3f17-119">**Hitelkártya száma** a tartalom felismerését szükséges további tájékoztatást a következő részben a cikkben: [Mi az érzékeny adattípusok keresse meg a hitelkártya száma](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="e3f17-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="e3f17-120">A beépített érzékeny információk különböző típusú cikke információ szükséges egyéb Újdonságok: [keressen Mi a bizalmas információk típusai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e3f17-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  