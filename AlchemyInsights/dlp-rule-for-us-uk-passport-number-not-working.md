---
title: Az Amerikai Egyesült államokbeli Passport-szám nem működött a DLP-szabály szerint
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679226"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="5f736-102">A DLP-US/UK-hu/UK Passport-számokkal kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="5f736-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="5f736-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="5f736-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5f736-104">**DLP-problémák az Amerikai Egyesült államokbeli Passport-számokkal**</span><span class="sxs-lookup"><span data-stu-id="5f736-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="5f736-105">Problémákat tapasztal az **adatvesztés-megelőzéssel (DLP)** , ha nem működik az **amerikai/brit útlevél számát** tartalmazó tartalom, ha a O365-ban DLP típusú bizalmas adattípust használ?</span><span class="sxs-lookup"><span data-stu-id="5f736-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="5f736-106">Ha igen, győződjön meg arról, hogy a tartalom a kiértékeléskor a DLP-házirend szempontjából szükséges információkat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="5f736-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="5f736-107">Például az 75%-os megbízhatósági szinttel konfigurált **amerikai/brit Passport** -házirend esetén a program kiértékeli az alábbiakat, és észleli a szabályt az indításhoz.</span><span class="sxs-lookup"><span data-stu-id="5f736-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="5f736-108">**[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Kilenc számjegy</span><span class="sxs-lookup"><span data-stu-id="5f736-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="5f736-109">**[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Kilenc egymást követő számjegy</span><span class="sxs-lookup"><span data-stu-id="5f736-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="5f736-110">**[Ellenőrzőösszeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nem, nincs ellenőrzőösszeg</span><span class="sxs-lookup"><span data-stu-id="5f736-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="5f736-111">**[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP-házirend 75%-os megbízhatósági szinttel jelenti az ilyen típusú bizalmas adatok észlelését, ha az 300 karaktereken belül:</span><span class="sxs-lookup"><span data-stu-id="5f736-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="5f736-112">A függvény Func_usa_uk_passport megkeresi a mintázattal egyező tartalmat.</span><span class="sxs-lookup"><span data-stu-id="5f736-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="5f736-113">A Keyword_passport kulcsszója megtalálható.</span><span class="sxs-lookup"><span data-stu-id="5f736-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="5f736-114">Az alábbi minta például az Amerikai Egyesült államokbeli **Passport-számokra** vonatkozó házirend: az Amerikai Egyesült államokbeli útlevél száma 123456789</span><span class="sxs-lookup"><span data-stu-id="5f736-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="5f736-115">Ha szeretne többet megtudni arról, hogy mire van szükség egy amerikai/brit Passport-számhoz a tartalomhoz, olvassa el a következő cikket: [Mi a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="5f736-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="5f736-116">Ha más beépített bizalmas adattípust használ, további információt a következő témakörben talál: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="5f736-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  