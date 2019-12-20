---
title: Csapatok 4c7 hibaüzenetet kapja hiba
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796168"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="53c42-102">4c7 hibaüzenetet kapja hiba a Microsoft csapatok</span><span class="sxs-lookup"><span data-stu-id="53c42-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="53c42-103">Ez a hiba azért jelentkezik, mert a Microsoft-csapatok űrlaphitelesítést igényel.</span><span class="sxs-lookup"><span data-stu-id="53c42-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="53c42-104">Az Active Directory összevonási szolgáltatások (AD FS) telepítésekor alapértelmezés szerint az űrlap-hitelesítés nincs engedélyezve az intraneten.</span><span class="sxs-lookup"><span data-stu-id="53c42-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="53c42-105">Ha az integrált Windows-hitelesítés sikertelen, a rendszer az űrlapos hitelesítés használatával kéri a bejelentkezést.</span><span class="sxs-lookup"><span data-stu-id="53c42-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="53c42-106">A probléma megoldásához engedélyezze az űrlapos hitelesítést az Active Directory összevonási szolgáltatások MMC beépülő moduljával azon a számítógépen, amelyen a helyi példány található.</span><span class="sxs-lookup"><span data-stu-id="53c42-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="53c42-107">Ehhez kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="53c42-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="53c42-108">A navigációs ablaktáblán tallózással keresse meg a **hitelesítési házirendeket**.</span><span class="sxs-lookup"><span data-stu-id="53c42-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="53c42-109">A részleteket tartalmazó ablaktábla **műveletek** csoportjában jelölje be a **globális elsődleges hitelesítés szerkesztése**választógombot.</span><span class="sxs-lookup"><span data-stu-id="53c42-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="53c42-110">Az **intranet** lapon jelölje be az **űrlapos hitelesítés**választógombot.</span><span class="sxs-lookup"><span data-stu-id="53c42-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="53c42-111">Válassza **az OK** (vagy **alkalmazás**)-t.</span><span class="sxs-lookup"><span data-stu-id="53c42-111">Select **OK** (or **Apply**).</span></span>