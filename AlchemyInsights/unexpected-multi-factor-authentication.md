---
title: Nem várt többtényezős hitelesítés
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: a664bd709062ec1335ebcf1f9adddc8aef917ac1
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766603"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="46b12-102">Nem várt többtényezős hitelesítés</span><span class="sxs-lookup"><span data-stu-id="46b12-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="46b12-103">Ha a bérlői fiókját a 2019. október 21. után hozták létre, és Önt váratlanul többtényezős hitelesítésre kérik, akkor a bérlői fiókban valószínűleg engedélyezték az [alapértelmezett biztonsági beállításokat](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="46b12-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="46b12-104">Az alapértelmezett biztonsági beállítások kezelése:</span><span class="sxs-lookup"><span data-stu-id="46b12-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="46b12-105">Jelentkezzen be a [felügyeleti központba](https://go.microsoft.com/fwlink/p/?linkid=834822) a globális rendszergazdai hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="46b12-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="46b12-106">Lépjen az [Azure Active Directory – Tulajdonságok](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties) lapra.</span><span class="sxs-lookup"><span data-stu-id="46b12-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="46b12-107">A lap alján válassza ki az **Alapértelmezett biztonsági beállítások kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="46b12-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="46b12-108">Válassza az **Igen** lehetőséget a biztonsági alapértékek engedélyezéséhez, és a **Nem** lehetőséget a biztonsági alapértékek letiltásához.</span><span class="sxs-lookup"><span data-stu-id="46b12-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
