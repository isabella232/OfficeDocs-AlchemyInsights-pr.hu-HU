---
title: GPO-telepítés
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427569"
---
# <a name="gpo-deployment"></a><span data-ttu-id="c6239-102">GPO-telepítés</span><span class="sxs-lookup"><span data-stu-id="c6239-102">GPO Deployment</span></span>

<span data-ttu-id="c6239-103">Az Azure Active Directory tartományi szolgáltatásokban (Azure AD DS) található felhasználói és számítógépes objektumok beállításait gyakran csoportházirend-objektumok (GPOs) használatával kezelik.</span><span class="sxs-lookup"><span data-stu-id="c6239-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="c6239-104">Az Azure AD DS beépített CSOPORTHÁZIREND-objektumokat tartalmaz az AADDC-felhasználók és az AADDC számítógépek tárolóihoz.</span><span class="sxs-lookup"><span data-stu-id="c6239-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="c6239-105">Ezeket a beépített csoportházirend-objektumokat testre szabhatja úgy, hogy a környezetéhez szükség szerint konfigurálja a csoportházirendeket.</span><span class="sxs-lookup"><span data-stu-id="c6239-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="c6239-106">Az Azure AD DC rendszergazdák csoportjának tagjai csoportházirend-felügyeleti jogosultságokkal az Azure AD DS tartományban, valamint egyéni csoportházirend-objektumokat és szervezeti egységeket is létrehozhatnak.</span><span class="sxs-lookup"><span data-stu-id="c6239-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="c6239-107">A csoportházirendek szerkezetét és működését a Csoportházirendek áttekintése [témakörben olvashatja.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="c6239-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="c6239-108">Hibrid környezetben a helyszíni AD DS-környezetben konfigurált csoportházirendek nem szinkronizálódnak az Azure AD DS szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="c6239-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="c6239-109">Ha konfigurációs beállításokat ad meg az Azure AD DS felhasználóinak vagy számítógépein, szerkessze az egyik alapértelmezett csoportházirend-objektumát, vagy hozzon létre egy egyéni csoportházirend-objektumát.</span><span class="sxs-lookup"><span data-stu-id="c6239-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="c6239-110">Ez a [csoportházirend-kezelésről](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) készült cikk bemutatja, hogy miként telepítheti a csoportházirend-kezelő eszközöket, hogyan módosíthatja a beépített csoportházirend-objektumokat, és hogyan hozhat létre egyéni csoportházirend-objektumokat.</span><span class="sxs-lookup"><span data-stu-id="c6239-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
