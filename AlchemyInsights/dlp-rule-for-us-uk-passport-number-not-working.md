---
title: DLP szabály az USA / UK útlevél száma nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389543"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="943b5-102">DLP - problémák US / UK Passport számok</span><span class="sxs-lookup"><span data-stu-id="943b5-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="943b5-103">Akkor problémák adódnak az **Adatok elvesztésének megakadályozása (DLP)** tartalmazó tartalom nem működik a **USA / UK útlevél száma** O365 a DLP érzékeny adatok típusa használatakor?</span><span class="sxs-lookup"><span data-stu-id="943b5-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="943b5-104">Ha igen, ellenőrizze, hogy a tartalom olvasható Mi a DLP házirendet keres, ha azt értékelje ki a szükséges adatokat.</span><span class="sxs-lookup"><span data-stu-id="943b5-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="943b5-105">Például, ha egy **US / UK útlevél száma** 75 %-os megbízhatósági szint konfigurált házirend, a következő értékelik, és fel kell deríteni a kiváltó szabály</span><span class="sxs-lookup"><span data-stu-id="943b5-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="943b5-106">**[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Kilenc számjegy</span><span class="sxs-lookup"><span data-stu-id="943b5-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="943b5-107">**[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Kilenc egymást követő számjegyből álló</span><span class="sxs-lookup"><span data-stu-id="943b5-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="943b5-108">**[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nem, nincs nincs ellenőrzőösszeg</span><span class="sxs-lookup"><span data-stu-id="943b5-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="943b5-109">**[Meghatározása:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP házirend abban, hogy ilyen jellegű érzékeny adatokat észlelt 75 %-át Ha a közelség 300 karakter belül:</span><span class="sxs-lookup"><span data-stu-id="943b5-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="943b5-110">A függvény Func_usa_uk_passport tartalom, amely megfelel a minta keresése.</span><span class="sxs-lookup"><span data-stu-id="943b5-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="943b5-111">A Keyword_passport kulcsszó található.</span><span class="sxs-lookup"><span data-stu-id="943b5-111">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="943b5-112">Például, indítsa el a következő minta esetében a **USA / UK útlevél száma** házirend: 123456789 amerikai útlevél száma</span><span class="sxs-lookup"><span data-stu-id="943b5-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="943b5-113">További információt az Egyesült Államok szükséges / UK útlevél száma felismerését a tartalom a következő részben az e cikkben: [Mi a bizalmas információ típusú keresés amerikai / UK útlevél száma](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="943b5-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="943b5-114">A beépített érzékeny információk különböző típusú cikke információ szükséges egyéb Újdonságok: [keressen Mi a bizalmas információk típusai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="943b5-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  