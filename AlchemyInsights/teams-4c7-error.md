---
title: Teams 4c7-es hiba
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786671"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="29a38-102">4c7-es hiba a Microsoft Teamsben</span><span class="sxs-lookup"><span data-stu-id="29a38-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="29a38-103">Ez a hiba azért jelenik meg, mert a Microsoft Teams űrlap-hitelesítést igényel.</span><span class="sxs-lookup"><span data-stu-id="29a38-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="29a38-104">Az Active Directory összevonási szolgáltatások (AD FS) telepítésekor az űrlap-hitelesítés alapértelmezés szerint nincs engedélyezve az intranethez.</span><span class="sxs-lookup"><span data-stu-id="29a38-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="29a38-105">Ha a Windows integrált hitelesítése nem sikerül, a rendszer kéri, hogy jelentkezzen be űrlap-hitelesítéssel.</span><span class="sxs-lookup"><span data-stu-id="29a38-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="29a38-106">A probléma megoldásához engedélyezze az Űrlap-hitelesítést az AD FS Microsoft Management Console (MMC) beépülő modul használatával az Active Directory helyi példányát használó számítógépen.</span><span class="sxs-lookup"><span data-stu-id="29a38-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="29a38-107">Ehhez hajtsa végre a következő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="29a38-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="29a38-108">A navigációs ablakban válassza a Hitelesítési **házirendek lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="29a38-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="29a38-109">A **részletek ablaktáblán** a Műveletek csoportban válassza a Globális elsődleges hitelesítés **szerkesztése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="29a38-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="29a38-110">Az **Intranet lapon** válassza az Űrlapok **hitelesítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="29a38-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="29a38-111">Válassza **az OK** (vagy az **Alkalmaz) gombot.**</span><span class="sxs-lookup"><span data-stu-id="29a38-111">Select **OK** (or **Apply**).</span></span>