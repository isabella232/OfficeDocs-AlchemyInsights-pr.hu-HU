---
title: Feltételes hozzáférési szabályzatok
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 8ce41d007988f2a45f1ded385ae50ac3def97c1b
ms.sourcegitcommit: 9923ce61344e22c4490549b12f65fa2896490b1f
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2020
ms.locfileid: "43100508"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="c7f15-102">Feltételes hozzáférési szabályzatok</span><span class="sxs-lookup"><span data-stu-id="c7f15-102">Conditional Access policies</span></span>

<span data-ttu-id="c7f15-103">A feltételes hozzáférés az Azure AD funkciója, amely lehetővé teszi a vezérlők kényszerítését a környezetében lévő appokhoz való hozzáféréshez, adott feltételek alapján és egy központi helyről felügyelve.</span><span class="sxs-lookup"><span data-stu-id="c7f15-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="c7f15-104">További információ az [Azure AD feltételes hozzáférés](https://docs.microsoft.com/azure/active-directory/conditional-access/) funkciójáról.</span><span class="sxs-lookup"><span data-stu-id="c7f15-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="c7f15-105">**Megjegyzés**: Ha bérlői fiókját 2019. október 21. után hozták létre, és Önt váratlanul többtényezős hitelesítésre kérik, akkor a bérlői fiókban valószínűleg engedélyezték az [alapértelmezett biztonsági beállításokat](http://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="c7f15-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="c7f15-106">**Az alapértelmezett biztonsági beállítások kezelése**</span><span class="sxs-lookup"><span data-stu-id="c7f15-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="c7f15-107">Jelentkezzen be a [felügyeleti központba](https://go.microsoft.com/fwlink/p/?linkid=834822) a globális rendszergazdai hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="c7f15-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="c7f15-108">Lépjen az [Azure Active Directory – Tulajdonságok](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties) lapra.</span><span class="sxs-lookup"><span data-stu-id="c7f15-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="c7f15-109">A lap alján válassza ki az **Alapértelmezett biztonsági beállítások kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c7f15-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="c7f15-110">Válassza az **Igen** lehetőséget a biztonsági alapértékek engedélyezéséhez, és a **Nem** lehetőséget a biztonsági alapértékek letiltásához.</span><span class="sxs-lookup"><span data-stu-id="c7f15-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
