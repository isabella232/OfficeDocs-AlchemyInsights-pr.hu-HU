---
title: Az amerikai bankszámlaszám nem mûködõ DLP-szabály
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679298"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="05ae1-102">DLP-problémák az amerikai bankszámlák számaival</span><span class="sxs-lookup"><span data-stu-id="05ae1-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="05ae1-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="05ae1-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="05ae1-104">**DLP-problémák az amerikai bankszámlák számaival**</span><span class="sxs-lookup"><span data-stu-id="05ae1-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="05ae1-105">Problémákat tapasztal az **adatvesztés-megelőzéssel (DLP)** , ha nem működik az **amerikai bankszámlaszám** tartalmazó tartalmaknál a O365-ban DLP típusú bizalmas adattípus használatakor?</span><span class="sxs-lookup"><span data-stu-id="05ae1-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="05ae1-106">Ha igen, győződjön meg arról, hogy a tartalom a kiértékeléskor a DLP-házirend szempontjából szükséges információkat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="05ae1-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="05ae1-107">Például az 85%-os megbízhatósági szinttel konfigurált **amerikai bankszámlaszám** -házirend esetén a program kiértékeli az alábbiakat, és a szabálynak a következőképpen kell kiértékelést végeznie:</span><span class="sxs-lookup"><span data-stu-id="05ae1-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="05ae1-108">**[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 számjegyek</span><span class="sxs-lookup"><span data-stu-id="05ae1-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="05ae1-109">**[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 egymást követő számjegyek.</span><span class="sxs-lookup"><span data-stu-id="05ae1-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="05ae1-110">**[Ellenőrzőösszeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nem, nincs ellenőrzőösszeg</span><span class="sxs-lookup"><span data-stu-id="05ae1-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="05ae1-111">**[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP-házirend 75%-os megbízhatósági szinttel jelenti az ilyen típusú bizalmas adatok észlelését, ha az 300 karaktereken belül:</span><span class="sxs-lookup"><span data-stu-id="05ae1-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="05ae1-112">A normál kifejezés Regex_usa_bank_account_number megkeresi a mintázatnak megfelelő tartalmat</span><span class="sxs-lookup"><span data-stu-id="05ae1-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="05ae1-113">A Keyword_usa_Bank_Account kulcsszója megtalálható.</span><span class="sxs-lookup"><span data-stu-id="05ae1-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="05ae1-114">A következő minta például az **amerikai bankszámlaszám** -házirend: a 78344011 fiók ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="05ae1-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="05ae1-115">Ha szeretne többet megtudni arról, hogy mire van szükség egy **amerikai bankszámlaszám** a tartalomhoz való felderítéséhez, olvassa el a jelen cikk következő szakaszát: [Mi a bizalmas adattípusok keresése az amerikai bankszámlák számát](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="05ae1-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="05ae1-116">Ha más beépített bizalmas adattípust használ, további információt a következő témakörben talál: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="05ae1-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  