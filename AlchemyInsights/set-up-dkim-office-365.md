---
title: A beállítási DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808709"
---
# <a name="setup-dkim"></a><span data-ttu-id="1949f-102">A beállítási DKIM</span><span class="sxs-lookup"><span data-stu-id="1949f-102">Setup DKIM</span></span>

<span data-ttu-id="1949f-103">[Itt](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)megtudhatja, hogy miként konfigurálhatja a DKIM az egyéni tartományokhoz a Microsoft 365-ban.</span><span class="sxs-lookup"><span data-stu-id="1949f-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="1949f-104">**Minden** egyéni tartományhoz létre kell hoznia **két** DKIM CNAME rekordot a tartomány DNS-szolgáltatójánál (általában a tartományregisztrálónál).</span><span class="sxs-lookup"><span data-stu-id="1949f-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="1949f-105">A contoso.com és a fourthcoffee.com például négy DKIM CNAME rekordot követel meg: kettőt a contoso.com és kettőt a fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="1949f-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="1949f-106">Az **egyes** egyéni tartományokhoz tartozó DKIM CNAME rekordjai a következő formátumokat használják:</span><span class="sxs-lookup"><span data-stu-id="1949f-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="1949f-107">**Host Name (állomásnév**): `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="1949f-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="1949f-108">Címzett **pont vagy érték**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="1949f-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="1949f-109">**TTL (TTL**): 3600</span><span class="sxs-lookup"><span data-stu-id="1949f-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="1949f-110">**Host Name (állomásnév**): `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="1949f-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="1949f-111">Címzett **pont vagy érték**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="1949f-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="1949f-112">**TTL (TTL**): 3600</span><span class="sxs-lookup"><span data-stu-id="1949f-112">**TTL**: 3600</span></span>

   <span data-ttu-id="1949f-113">\<DomainGUID\> az `.mail.protection.outlook.com` Egyéni tartományhoz tartozó egyéni MX rekordtól balra lévő szöveg (például `contoso-com` a tartomány contoso.com).</span><span class="sxs-lookup"><span data-stu-id="1949f-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="1949f-114">\<InitialDomain\> a Microsoft 365-ra való regisztrációkor használt tartomány (például contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="1949f-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="1949f-115">Miután létrehozta a CNAME rekordokat az egyéni tartományokhoz, kövesse az alábbi utasításokat:</span><span class="sxs-lookup"><span data-stu-id="1949f-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="1949f-116">a.</span><span class="sxs-lookup"><span data-stu-id="1949f-116">a.</span></span> <span data-ttu-id="1949f-117">[Bejelentkezés a Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) a munkahelyi vagy iskolai fiókjával.</span><span class="sxs-lookup"><span data-stu-id="1949f-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="1949f-118">b.</span><span class="sxs-lookup"><span data-stu-id="1949f-118">b.</span></span> <span data-ttu-id="1949f-119">Kattintson az appindító ikonra a bal felső sarokban, és kattintson a **Rendszergazda** elemre.</span><span class="sxs-lookup"><span data-stu-id="1949f-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="1949f-120">c.</span><span class="sxs-lookup"><span data-stu-id="1949f-120">c.</span></span> <span data-ttu-id="1949f-121">A bal oldali navigációs sávon bontsa ki a **rendszergazda** csomópontot, és válassza az **Exchange**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1949f-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="1949f-122">d.</span><span class="sxs-lookup"><span data-stu-id="1949f-122">d.</span></span> <span data-ttu-id="1949f-123">Nyissa meg a **védelmi**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="1949f-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="1949f-124">e.</span><span class="sxs-lookup"><span data-stu-id="1949f-124">e.</span></span> <span data-ttu-id="1949f-125">Jelölje ki a tartományt, és válassza az **Engedélyezés** lehetőséget a **tartomány DKIM aláírásokkal való aláírásához**.</span><span class="sxs-lookup"><span data-stu-id="1949f-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="1949f-126">Ismételje meg ezt a lépést mindegyik egyéni tartománynál.</span><span class="sxs-lookup"><span data-stu-id="1949f-126">Repeat this step for each custom domain.</span></span>
