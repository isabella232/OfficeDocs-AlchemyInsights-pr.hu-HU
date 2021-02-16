---
title: Csoportházirend
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256778"
---
# <a name="group-policy"></a><span data-ttu-id="69e69-102">Csoportházirend</span><span class="sxs-lookup"><span data-stu-id="69e69-102">Group policy</span></span>

<span data-ttu-id="69e69-103">Az Azure Active Directory tartományi szolgáltatásokban (Azure AD DS) lévő felhasználói és számítógépes objektumok beállításait gyakran csoportházirend-objektumok (GPOs) használatával kezelik.</span><span class="sxs-lookup"><span data-stu-id="69e69-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="69e69-104">Az Azure AD DS beépített CSOPORTHÁZIREND-objektumokat tartalmaz az AADDC-felhasználók és az AADDC számítógépek tárolóihoz.</span><span class="sxs-lookup"><span data-stu-id="69e69-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="69e69-105">Ezeket a beépített csoportházirend-objektumokat testre szabhatja úgy, hogy a környezetéhez szükség szerint konfigurálja a csoportházirendeket.</span><span class="sxs-lookup"><span data-stu-id="69e69-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="69e69-106">Az Azure AD DC rendszergazdák csoportjának tagjai csoportházirend-felügyeleti jogosultságokkal az Azure AD DS tartományban, valamint egyéni csoportházirend-objektumokat és szervezeti egységeket is létrehozhatnak.</span><span class="sxs-lookup"><span data-stu-id="69e69-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="69e69-107">A csoportházirendek szerkezetét és működését a Csoportházirend áttekintése [témakörben olvashatja.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="69e69-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="69e69-108">Hibrid környezetben a helyszíni AD DS-környezetben konfigurált csoportházirendek nem szinkronizálódnak az Azure AD DS szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="69e69-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="69e69-109">Ha konfigurációs beállításokat ad meg az Azure AD DS felhasználóinak vagy számítógépein, szerkessze az egyik alapértelmezett csoportházirend-objektumát, vagy hozzon létre egy egyéni csoportházirend-objektumát.</span><span class="sxs-lookup"><span data-stu-id="69e69-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="69e69-110">Ez a cikk a [csoportházirendek](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) kezelését mutatja be, hogy miként telepítheti a csoportházirend-kezelő eszközöket, hogyan módosíthatja a beépített csoportházirend-objektumokat, és hogyan hozhat létre egyéni csoportházirend-objektumokat.</span><span class="sxs-lookup"><span data-stu-id="69e69-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



