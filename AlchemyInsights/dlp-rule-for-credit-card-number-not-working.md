---
title: Nem működött a hitelkártya-számhoz tartozó DLP-szabály
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679443"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="a7ef0-102">DLP-problémák a hitelkártya-számokkal</span><span class="sxs-lookup"><span data-stu-id="a7ef0-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="a7ef0-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="a7ef0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a7ef0-104">**DLP-problémák a hitelkártya-számokkal**</span><span class="sxs-lookup"><span data-stu-id="a7ef0-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="a7ef0-105">Problémát tapasztal az **adatvesztés-megelőzéssel (DLP)** kapcsolatban, ha nem működik a **hitelkártyát** tartalmazó tartalom, ha a O365-ban DLP típusú bizalmas adattípust használ?</span><span class="sxs-lookup"><span data-stu-id="a7ef0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a7ef0-106">Ha igen, gondoskodjon arról, hogy a tartalom a kiértékeléskor a DLP-házirend elindításához szükséges információkat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="a7ef0-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="a7ef0-107">A 85%-os megbízhatósági szinttel konfigurált **hitelkártya-házirend** esetén például a program kiértékeli az alábbiakat, és a következőhöz kell észlelni:</span><span class="sxs-lookup"><span data-stu-id="a7ef0-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a7ef0-108">**[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 számjegy, amely formázható vagy formázható (közönséges számsorozatként), és meg kell adnia a Luhn tesztet.</span><span class="sxs-lookup"><span data-stu-id="a7ef0-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="a7ef0-109">**[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Nagyon bonyolult és robusztus minta, amely az egész világon elérhető főbb márkák kártyáit észleli, többek között Visa, MasterCard, Discover Card, JCB, American Express, Gift Cards és Diner kártyával.</span><span class="sxs-lookup"><span data-stu-id="a7ef0-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="a7ef0-110">**[Ellenőrzőösszeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Igen, az Luhn ellenőrzőösszeg</span><span class="sxs-lookup"><span data-stu-id="a7ef0-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="a7ef0-111">**[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP-házirend 85%-os megbízhatósági szinttel jelenti az ilyen típusú bizalmas adatok észlelését, ha az 300 karaktereken belül:</span><span class="sxs-lookup"><span data-stu-id="a7ef0-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a7ef0-112">A függvény Func_credit_card megkeresi a mintázattal egyező tartalmat.</span><span class="sxs-lookup"><span data-stu-id="a7ef0-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a7ef0-113">Az alábbiak egyike igaz:</span><span class="sxs-lookup"><span data-stu-id="a7ef0-113">One of the following is true:</span></span>

  - <span data-ttu-id="a7ef0-114">A Keyword_cc_verification kulcsszója megtalálható.</span><span class="sxs-lookup"><span data-stu-id="a7ef0-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="a7ef0-115">Keyword_cc_name található kulcsszó</span><span class="sxs-lookup"><span data-stu-id="a7ef0-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="a7ef0-116">A függvény Func_expiration_date a megfelelő dátum formátumban keresi a dátumot.</span><span class="sxs-lookup"><span data-stu-id="a7ef0-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="a7ef0-117">Az ellenőrzőösszeg áthalad</span><span class="sxs-lookup"><span data-stu-id="a7ef0-117">The checksum passes</span></span>

    <span data-ttu-id="a7ef0-118">Az alábbi példa például egy DLP-beli hitelkártya-házirendet indít el:</span><span class="sxs-lookup"><span data-stu-id="a7ef0-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="a7ef0-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="a7ef0-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="a7ef0-120">Lejárat: 2/2009</span><span class="sxs-lookup"><span data-stu-id="a7ef0-120">Expires: 2/2009</span></span>

<span data-ttu-id="a7ef0-121">Ha többet szeretne megtudni arról, hogy mire van szüksége a tartalomhoz a **hitelkártyaszám** felderítéséhez, olvassa el a következő cikket: [Mi a bizalmas adattípusok keresése a hitelkártyával #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="a7ef0-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="a7ef0-122">Ha más beépített bizalmas adattípust használ, további információt a következő témakörben talál: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="a7ef0-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  