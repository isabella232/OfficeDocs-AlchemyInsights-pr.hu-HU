---
title: A telepítő az Office 365 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666266"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="99090-102">A telepítő az Office 365 DKIM</span><span class="sxs-lookup"><span data-stu-id="99090-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="99090-103">DKIM konfigurálása az Office 365 rendszerben egyéni tartományokat a teljes körű útmutatást talál [Itt](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="99090-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="99090-104">**Minden** egyéni tartományhoz kell létrehozni **két** DKIM CNAME rekordot a tartomány DNS-üzemeltetési szolgáltatást (általában a tartomány hivatalvezető).</span><span class="sxs-lookup"><span data-stu-id="99090-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="99090-105">Például, contoso.com és fourthcoffee.com szükséges négy DKIM CNAME rekordok: két, contoso.com és kettő fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="99090-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="99090-106">**Minden** egyéni tartomány DKIM CNAME rekordok használata a következő formátumokban:</span><span class="sxs-lookup"><span data-stu-id="99090-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="99090-107">**Állomás neve**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="99090-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="99090-108">**Cím vagy értéket mutat**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="99090-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="99090-109">**Élettartam**: 3600</span><span class="sxs-lookup"><span data-stu-id="99090-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="99090-110">**Állomás neve**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="99090-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="99090-111">**Cím vagy értéket mutat**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="99090-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="99090-112">**Élettartam**: 3600</span><span class="sxs-lookup"><span data-stu-id="99090-112">**TTL**: 3600</span></span>

   <span data-ttu-id="99090-113">\<DomainGUID\> a szöveg a bal oldali `.mail.protection.outlook.com` a testreszabott MX rekord az egyéni tartomány (például `contoso-com` az a tartomány contoso.com).</span><span class="sxs-lookup"><span data-stu-id="99090-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="99090-114">\<InitialDomain\> az Office 365 (például contoso.onmicrosoft.com) való regisztráció során használt tartomány.</span><span class="sxs-lookup"><span data-stu-id="99090-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="99090-115">Miután létrehozta a CNAME rekordok az egyéni tartományok, hajtsa végre az alábbi utasításokat:</span><span class="sxs-lookup"><span data-stu-id="99090-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="99090-116">egy.</span><span class="sxs-lookup"><span data-stu-id="99090-116">a.</span></span> <span data-ttu-id="99090-117">[Jelentkezzen be az Office 365-be](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) munkahelyi vagy iskolai fiók segítségével.</span><span class="sxs-lookup"><span data-stu-id="99090-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="99090-118">b.</span><span class="sxs-lookup"><span data-stu-id="99090-118">b.</span></span> <span data-ttu-id="99090-119">Kattintson az alkalmazásindító ikonra a bal felső sarokban, és kattintson a **Rendszergazda** elemre.</span><span class="sxs-lookup"><span data-stu-id="99090-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="99090-120">c.</span><span class="sxs-lookup"><span data-stu-id="99090-120">c.</span></span> <span data-ttu-id="99090-121">A bal alsó navigációs bontsa ki az **Admin** , és válassza az **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="99090-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="99090-122">d.</span><span class="sxs-lookup"><span data-stu-id="99090-122">d.</span></span> <span data-ttu-id="99090-123">Ugrás a **védelem** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="99090-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="99090-124">e.</span><span class="sxs-lookup"><span data-stu-id="99090-124">e.</span></span> <span data-ttu-id="99090-125">Jelölje ki a tartományt és válassza **engedélyezése** **bejelentkezési**üzenet a DKIM aláírást tartalmazó tartomány.</span><span class="sxs-lookup"><span data-stu-id="99090-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="99090-126">Ismételje meg ezt a lépést minden egyéni tartomány.</span><span class="sxs-lookup"><span data-stu-id="99090-126">Repeat this step for each custom domain.</span></span>
