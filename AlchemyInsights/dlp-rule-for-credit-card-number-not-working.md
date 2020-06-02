---
title: DLP-szabály a hitelkártyaszám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507408"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="2721f-102">DLP-problémák hitelkártyaszámokkal</span><span class="sxs-lookup"><span data-stu-id="2721f-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="2721f-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="2721f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2721f-104">**DLP-problémák hitelkártyaszámokkal**</span><span class="sxs-lookup"><span data-stu-id="2721f-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="2721f-105">Problémái vannak azzal, hogy **az Adatveszteség-megelőzés (DLP)** nem működik a **hitelkártyaszámot** tartalmazó tartalom esetében, amikor Az O365-ben DLP-érzékeny információtípust használ?</span><span class="sxs-lookup"><span data-stu-id="2721f-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2721f-106">Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat a DLP-házirend aktiválásához a kiértékeléskor.</span><span class="sxs-lookup"><span data-stu-id="2721f-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="2721f-107">A 85%-os megbízhatósági szinttel konfigurált **hitelkártya-házirendek** esetében például a rendszer a következőket értékeli ki, és a szabály aktiválásához észlelni kell őket:</span><span class="sxs-lookup"><span data-stu-id="2721f-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2721f-108">**[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 számjegy, amely formázható vagy formázható (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="2721f-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="2721f-109">**[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Nagyon összetett és robusztus minta, amely észleli a világ összes jelentős márkájának kártyáit, beleértve a Visa, MasterCard, Discover Card, JCB, American Express, ajándékkártyákat és étkezőkártyákat.</span><span class="sxs-lookup"><span data-stu-id="2721f-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="2721f-110">**[Ellenőrző összeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Igen, a Luhn ellenőrző összeg</span><span class="sxs-lookup"><span data-stu-id="2721f-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="2721f-111">**[Meghatározás:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP-házirend 85%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:</span><span class="sxs-lookup"><span data-stu-id="2721f-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2721f-112">A Func_credit_card függvény a mintának megfelelő tartalmat talál.</span><span class="sxs-lookup"><span data-stu-id="2721f-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="2721f-113">Az alábbiak egyike igaz:</span><span class="sxs-lookup"><span data-stu-id="2721f-113">One of the following is true:</span></span>

  - <span data-ttu-id="2721f-114">A Keyword_cc_verification kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="2721f-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="2721f-115">A Keyword_cc_name kulcsszó található</span><span class="sxs-lookup"><span data-stu-id="2721f-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="2721f-116">A Func_expiration_date függvény a megfelelő dátumformátumban keresi a dátumot.</span><span class="sxs-lookup"><span data-stu-id="2721f-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="2721f-117">Az ellenőrző összeg átmegy</span><span class="sxs-lookup"><span data-stu-id="2721f-117">The checksum passes</span></span>

    <span data-ttu-id="2721f-118">Például a következő minta a DLP hitelkártyaszám-házirendjének aktiválásához lépki:</span><span class="sxs-lookup"><span data-stu-id="2721f-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="2721f-119">Vízum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="2721f-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="2721f-120">Lejár: 2/2009</span><span class="sxs-lookup"><span data-stu-id="2721f-120">Expires: 2/2009</span></span>

<span data-ttu-id="2721f-121">Ha többet szeretne tudni arról, hogy mi szükséges a **hitelkártyaszám** észleléséhez a tartalomhoz, olvassa el a cikk következő szakaszát: [Milyen bizalmas információtípusok keresnek hitelkártyát#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="2721f-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="2721f-122">Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="2721f-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  