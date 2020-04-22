---
title: DKIM beállítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645674"
---
# <a name="setup-dkim"></a><span data-ttu-id="9aa52-102">DKIM beállítása</span><span class="sxs-lookup"><span data-stu-id="9aa52-102">Setup DKIM</span></span>

<span data-ttu-id="9aa52-103">A Microsoft 365-ben az egyéni tartományokhoz való DKIM-konfigurálásának teljes útmutatója [itt](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)található.</span><span class="sxs-lookup"><span data-stu-id="9aa52-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="9aa52-104">**Minden** egyéni tartományhoz **két** DKIM CNAME rekordot kell létrehoznia a tartomány DNS-szolgáltatószolgáltatásában (általában a tartományregisztrálónál).</span><span class="sxs-lookup"><span data-stu-id="9aa52-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="9aa52-105">Contoso.com és fourthcoffee.com például négy DKIM CNAME rekordot igényel: kettőt contoso.com és kettőt fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="9aa52-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="9aa52-106">Az **egyes** egyéni tartományok DKIM CNAME rekordjai a következő formátumokat használják:</span><span class="sxs-lookup"><span data-stu-id="9aa52-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="9aa52-107">**Állomásneve**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9aa52-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9aa52-108">**Címre vagy értékre mutat:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9aa52-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9aa52-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9aa52-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="9aa52-110">**Állomásneve**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9aa52-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9aa52-111">**Címre vagy értékre mutat:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9aa52-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9aa52-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9aa52-112">**TTL**: 3600</span></span>

   <span data-ttu-id="9aa52-113">\<A DomainGUID\> az egyéni `.mail.protection.outlook.com` tartomány testreszabott MX rekordjában (például `contoso-com` a tartomány contoso.com) bal oldalán lévő szöveg.</span><span class="sxs-lookup"><span data-stu-id="9aa52-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="9aa52-114">\<InitialDomain\> az a tartomány, amelyet a Microsoft 365-re való feliratkozáskor használt (például contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="9aa52-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="9aa52-115">Miután létrehozta az egyéni tartományok CNAME rekordjait, hajtsa végre az alábbi utasításokat:</span><span class="sxs-lookup"><span data-stu-id="9aa52-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="9aa52-116">A.</span><span class="sxs-lookup"><span data-stu-id="9aa52-116">a.</span></span> <span data-ttu-id="9aa52-117">[jelentkezzen be a Microsoft 365-be](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) munkahelyi vagy iskolai fiókjával.</span><span class="sxs-lookup"><span data-stu-id="9aa52-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="9aa52-118">B.</span><span class="sxs-lookup"><span data-stu-id="9aa52-118">b.</span></span> <span data-ttu-id="9aa52-119">Kattintson az appindító ikonra a bal felső sarokban, és kattintson a **Rendszergazda** elemre.</span><span class="sxs-lookup"><span data-stu-id="9aa52-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="9aa52-120">C.</span><span class="sxs-lookup"><span data-stu-id="9aa52-120">c.</span></span> <span data-ttu-id="9aa52-121">A bal alsó navigációs sávon **bontsa** ki a Rendszergazda csomópontot, és válassza az **Exchange**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="9aa52-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="9aa52-122">D.</span><span class="sxs-lookup"><span data-stu-id="9aa52-122">d.</span></span> <span data-ttu-id="9aa52-123">Tovább a **Védelmi** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="9aa52-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="9aa52-124">E.</span><span class="sxs-lookup"><span data-stu-id="9aa52-124">e.</span></span> <span data-ttu-id="9aa52-125">Jelölje ki a tartományt, majd válassza az **Engedélyezés** **ehhez a tartományhoz dkim-aláírásokkal**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="9aa52-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="9aa52-126">Ismételje meg ezt a lépést minden egyéni tartományesetében.</span><span class="sxs-lookup"><span data-stu-id="9aa52-126">Repeat this step for each custom domain.</span></span>
