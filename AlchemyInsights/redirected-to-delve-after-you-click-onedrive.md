---
title: A OneDrive vállalati verzió webes OneDrive átirányítja a ásni-ra
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
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776381"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="d3db9-102">Átirányítva ás a OneDrive kattintás után</span><span class="sxs-lookup"><span data-stu-id="d3db9-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="d3db9-103">Részletes [hibaelhárítási útmutatót](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)talál.</span><span class="sxs-lookup"><span data-stu-id="d3db9-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="d3db9-104">A probléma megoldásához a rendszergazdának meg kell adnia a megfelelő jogosultságot a saját webhelyek webhely létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="d3db9-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="d3db9-105">Ennek az az oka, hogy a OneDrive vállalati verzió lap jön létre a saját webhelyeken.</span><span class="sxs-lookup"><span data-stu-id="d3db9-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="d3db9-106">A jogosultság megadásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="d3db9-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="d3db9-107">A SharePoint felügyeleti központban kattintson a **felhasználói profilok**elemre.</span><span class="sxs-lookup"><span data-stu-id="d3db9-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="d3db9-108">A **személyek** csoportban kattintson a **felhasználói engedélyek kezelése**elemre.</span><span class="sxs-lookup"><span data-stu-id="d3db9-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="d3db9-109">Adjon hozzá olyan felhasználókat, akiknek engedélyt kell adni a saját webhelyek webhelyének létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="d3db9-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="d3db9-110">Alapértelmezés szerint ez a beállítás a **külső felhasználók kivételével mindenki számára**beállításra van állítva.</span><span class="sxs-lookup"><span data-stu-id="d3db9-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="d3db9-111">Miután hozzáadta a felhasználót, felhasználókat vagy csoportot, győződjön meg arról, hogy a hozzáadott felhasználó, felhasználók vagy csoport van kijelölve, és jelölje be az **engedélyek** szakasz jelölőnégyzetét, és jelölje be a **személyes webhely létrehozása (a személyes tárterület, a hírcsatorna és a követett tartalom esetében szükséges)** jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="d3db9-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="d3db9-112">Kattintson az **OK gombra**, majd a felhasználó tallózással keresse meg a OneDrive lapot a webhely létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="d3db9-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
