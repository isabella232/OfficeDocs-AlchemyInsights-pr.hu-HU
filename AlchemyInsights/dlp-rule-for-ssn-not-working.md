---
title: Nem működött a SSN szabály
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679371"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="ec02f-102">A társadalombiztosítási számokkal kapcsolatos DLP-problémák</span><span class="sxs-lookup"><span data-stu-id="ec02f-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="ec02f-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="ec02f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ec02f-104">**DLP-problémák a azonosítókat keresi.-ban**</span><span class="sxs-lookup"><span data-stu-id="ec02f-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="ec02f-105">Problémát tapasztal az **adatvesztés-megelőzéssel (DLP)** kapcsolatban, ha nem működik a **társadalombiztosítási szám (SSN)** tartalmú tartalom a Microsoft 365 bizalmas adattípusa használatakor?</span><span class="sxs-lookup"><span data-stu-id="ec02f-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="ec02f-106">Ha igen, győződjön meg arról, hogy a tartalom a DLP-házirend kinézetéhez szükséges információkat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="ec02f-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="ec02f-107">Egy 85%-os megbízhatósági szinttel konfigurált SSN-házirend esetében például a program kiértékeli a következőt, és a következőhöz kell észlelni:</span><span class="sxs-lookup"><span data-stu-id="ec02f-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="ec02f-108">**[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 számjegy, amelyek formázott vagy formázatlan mintázatként jelenhetnek meg</span><span class="sxs-lookup"><span data-stu-id="ec02f-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="ec02f-109">**[Minta:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Négy függvény a azonosítókat keresi. keres négy különböző mintázatban:</span><span class="sxs-lookup"><span data-stu-id="ec02f-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="ec02f-110">A Func_ssn megkeresi a 2011-os erős formázást, amely szaggatott vagy szóköz formátumú (DDD-dd-azonosítókat keresi. vagy DDD dd-vel) van formázva.</span><span class="sxs-lookup"><span data-stu-id="ec02f-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="ec02f-111">A Func_unformatted_ssn olyan erős formázással 2011 rendelkező azonosítókat keresi. keres, amelyek nem formázottak kilenc egymást követő számjegyként (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="ec02f-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="ec02f-112">A Func_randomized_formatted_ssn a gondolatjelekkel vagy szóközökkel formázott 2011-azonosítókat keresi. (DDD-DD-vagy DDD dd)</span><span class="sxs-lookup"><span data-stu-id="ec02f-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="ec02f-113">A Func_randomized_unformatted_ssn megkeresi a 2011 azonosítókat keresi., amelyek nem formázottak kilenc egymást követő számjegyet (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="ec02f-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="ec02f-114">**[Ellenőrzőösszeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nem, nincs ellenőrzőösszeg</span><span class="sxs-lookup"><span data-stu-id="ec02f-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="ec02f-115">**[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP-házirend 85%-os megbízhatósági szinttel jelenti az ilyen típusú bizalmas adatok észlelését, ha az 300 karaktereken belül:</span><span class="sxs-lookup"><span data-stu-id="ec02f-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ec02f-116">A [függvény Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) megkeresi a mintázattal egyező tartalmat.</span><span class="sxs-lookup"><span data-stu-id="ec02f-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ec02f-117">A [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) kulcsszója megtalálható.</span><span class="sxs-lookup"><span data-stu-id="ec02f-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="ec02f-118">A kulcsszavak példái a következők:  *társadalombiztosítási, társadalombiztosítási #, SoC sec, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="ec02f-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="ec02f-119">Az alábbi példa például a DLP SSN-házirendet eredményezte: **ssn: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="ec02f-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="ec02f-120">Ha további információra van szüksége a azonosítókat keresi. a tartalomhoz való észleléséhez, olvassa el a jelen cikk következő szakaszát: [Mi a bizalmas adattípusok keresése a azonosítókat keresi.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) -ban</span><span class="sxs-lookup"><span data-stu-id="ec02f-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="ec02f-121">Ha más beépített bizalmas adattípust használ, további információt a következő témakörben talál: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="ec02f-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  