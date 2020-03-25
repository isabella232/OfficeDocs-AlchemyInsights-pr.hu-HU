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
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946743"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="62b20-102">Nem várt többtényezős hitelesítés</span><span class="sxs-lookup"><span data-stu-id="62b20-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="62b20-103">Ha a bérlői fiókját a 2019. október 21. után hozták létre, és Önt váratlanul többtényezős hitelesítésre kérik, akkor a bérlői fiókban valószínűleg engedélyezték az [alapértelmezett biztonsági beállításokat](http://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="62b20-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="62b20-104">Az alapértelmezett biztonsági beállítások kezelése:</span><span class="sxs-lookup"><span data-stu-id="62b20-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="62b20-105">Jelentkezzen be a [felügyeleti központba](https://go.microsoft.com/fwlink/p/?linkid=834822) a globális rendszergazdai hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="62b20-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="62b20-106">Lépjen az [Azure Active Directory – Tulajdonságok](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties) lapra.</span><span class="sxs-lookup"><span data-stu-id="62b20-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="62b20-107">A lap alján válassza ki az **Alapértelmezett biztonsági beállítások kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="62b20-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="62b20-108">Válassza az **Igen** lehetőséget a biztonsági alapértékek engedélyezéséhez, és a **Nem** lehetőséget a biztonsági alapértékek letiltásához.</span><span class="sxs-lookup"><span data-stu-id="62b20-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
