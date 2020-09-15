---
title: A Teams 4c7 hibaüzenetet kapja hibája
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700205"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="b1c1b-102">4c7 hibaüzenetet kapja hiba a Microsoft Teams alkalmazásban</span><span class="sxs-lookup"><span data-stu-id="b1c1b-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="b1c1b-103">Ez a hiba azért fordul elő, mert a Microsoft Teams űrlap-hitelesítést követel meg.</span><span class="sxs-lookup"><span data-stu-id="b1c1b-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="b1c1b-104">Ha telepíti az Active Directory összevonási szolgáltatásokat (AD FS), az űrlapos hitelesítés alapértelmezés szerint nincs engedélyezve az intraneten.</span><span class="sxs-lookup"><span data-stu-id="b1c1b-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="b1c1b-105">Ha a Windows beépített hitelesítése nem sikerült, a rendszer az űrlapos hitelesítéssel kéri a bejelentkezést.</span><span class="sxs-lookup"><span data-stu-id="b1c1b-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="b1c1b-106">A probléma megoldásához engedélyezze az űrlap-hitelesítést az AD FS Microsoft Management Console (MMC) beépülő modullal, amelyen az Active Directory helyi példánya található.</span><span class="sxs-lookup"><span data-stu-id="b1c1b-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="b1c1b-107">Ehhez hajtsa végre a következő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="b1c1b-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="b1c1b-108">A navigációs ablakban tallózással keresse meg a **hitelesítési szabályokat**.</span><span class="sxs-lookup"><span data-stu-id="b1c1b-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="b1c1b-109">A részletek ablaktábla **műveletek** csoportjában válassza a **globális elsődleges hitelesítés szerkesztése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b1c1b-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="b1c1b-110">Az **intranet** lapon válassza az **űrlapos hitelesítés**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b1c1b-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="b1c1b-111">Kattintson **az OK gombra** (vagy az **alkalmaz**gombra).</span><span class="sxs-lookup"><span data-stu-id="b1c1b-111">Select **OK** (or **Apply**).</span></span>