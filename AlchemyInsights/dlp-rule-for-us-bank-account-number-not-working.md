---
title: DLP szabály Nekünk bankszámla száma nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529871"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="d5ffa-102">US bankszámlaszámok DLP problémái</span><span class="sxs-lookup"><span data-stu-id="d5ffa-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="d5ffa-103">Hogy problémák adódnak az **Adatok elvesztésének megakadályozása (DLP)** tartalom **USA bankszámla számát** tartalmazó O365 a DLP érzékeny adatok típusa használatakor nem működik?</span><span class="sxs-lookup"><span data-stu-id="d5ffa-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d5ffa-104">Ha igen, ellenőrizze, hogy a tartalom olvasható Mi a DLP házirendet keres, ha azt értékelje ki a szükséges adatokat.</span><span class="sxs-lookup"><span data-stu-id="d5ffa-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d5ffa-105">Például **Amerikai bankszámlaszám** házirend konfigurálva 85 %-os megbízhatósági szint, a következő értékelik, és fel kell deríteni a kiváltó szabály:</span><span class="sxs-lookup"><span data-stu-id="d5ffa-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d5ffa-106">**[Formátuma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 számjegy</span><span class="sxs-lookup"><span data-stu-id="d5ffa-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="d5ffa-107">**[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** egymást követő számjegyből álló 8-17.</span><span class="sxs-lookup"><span data-stu-id="d5ffa-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="d5ffa-108">**[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nem, nincs nincs ellenőrzőösszeg</span><span class="sxs-lookup"><span data-stu-id="d5ffa-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d5ffa-109">**[Meghatározása:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP házirend abban, hogy ilyen jellegű érzékeny adatokat észlelt 75 %-át Ha a közelség 300 karakter belül:</span><span class="sxs-lookup"><span data-stu-id="d5ffa-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d5ffa-110">A reguláris kifejezés Regex_usa_bank_account_number tartalom, amely megfelel a minta keresése</span><span class="sxs-lookup"><span data-stu-id="d5ffa-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="d5ffa-111">A Keyword_usa_Bank_Account kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="d5ffa-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="d5ffa-112">Például, indítsa el a következő minta az **Egyesült Államok bankszámlaszám** házirend: folyószámla 78344011</span><span class="sxs-lookup"><span data-stu-id="d5ffa-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="d5ffa-113">**USA bankszámla szám** állapítható meg a tartalom szükséges további tájékoztatást a következő részben a cikkben: [Mi az érzékeny adattípusok USA bankszámla szám keresése](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="d5ffa-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="d5ffa-114">A beépített érzékeny információk különböző típusú cikke információ szükséges egyéb Újdonságok: [keressen Mi a bizalmas információk típusai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d5ffa-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  