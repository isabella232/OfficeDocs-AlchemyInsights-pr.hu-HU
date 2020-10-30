---
title: Bejelentkezés letiltása minden felhasználó számára
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003536"
- "6445"
ms.openlocfilehash: b1596fdf463413a5b6714c48f4097e9552948070
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807451"
---
# <a name="block-sign-in-for-all-users"></a><span data-ttu-id="c879f-102">Bejelentkezés letiltása minden felhasználó számára</span><span class="sxs-lookup"><span data-stu-id="c879f-102">Block sign in for all users</span></span>

<span data-ttu-id="c879f-103">Ha mindenkit le szeretne tiltani az Office-ba való bejelentkezésről, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="c879f-103">To block everyone from signing into Office, follow these steps:</span></span>

1. <span data-ttu-id="c879f-104">A felügyeleti központban nyissa meg a [ **felhasználók**  >  **aktív felhasználóit**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="c879f-104">In the admin center, go to [**Users** > **Active users**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
2. <span data-ttu-id="c879f-105">Az összes felhasználó kijelölése: jelölje be a **megjelenítendő név** melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="c879f-105">Select all users by clicking the check mark next to **Display Name** .</span></span> <span data-ttu-id="c879f-106">Ügyeljen arra, hogy törölje a bejelentkezett rendszergazdai fiók jelölőnégyzetét.</span><span class="sxs-lookup"><span data-stu-id="c879f-106">Ensure you uncheck the admin account you are logged in with.</span></span>
3. <span data-ttu-id="c879f-107">Kattintson a **"..."** elemre a **felhasználók exportálása** a  >  **bejelentkezési állapot szerkesztése** elem mellett, majd válassza **a felhasználók letiltása a bejelentkezéskor** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c879f-107">Click **"..."** next to **Export Users** > **Edit sign-in status** , then select **Block users from signing in** .</span></span> <span data-ttu-id="c879f-108">Az új bejelentkezések azonnal le vannak tiltva.</span><span class="sxs-lookup"><span data-stu-id="c879f-108">The new sign-ins are blocked immediately.</span></span> <span data-ttu-id="c879f-109">Ha egy felhasználó már be van jelentkezve, akkor a felhasználó a 60 percen belül automatikusan kijelentkezik az összes Microsoft-szolgáltatásból.</span><span class="sxs-lookup"><span data-stu-id="c879f-109">If a user was already signed in, then the user will be automatically signed out from all Microsoft services within 60 minutes.</span></span>
