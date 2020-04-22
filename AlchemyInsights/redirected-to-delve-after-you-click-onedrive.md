---
title: A OneDrive Vállalati verzió Web OneDrive átirányítása a Delve-re
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722812"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="c3ec5-102">Átirányítva a Delve-re, miután a OneDrive-ra kattintott</span><span class="sxs-lookup"><span data-stu-id="c3ec5-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="c3ec5-103">Tekintse meg részletes [hibaelhárítási útmutatónkat.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="c3ec5-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="c3ec5-104">A probléma megoldásához a rendszergazdának fel kell adnia a felhasználóknak a jogot a Saját helyek webhely ük létrehozására.</span><span class="sxs-lookup"><span data-stu-id="c3ec5-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="c3ec5-105">Ennek az az oka, hogy a OneDrive Vállalati verzió lap a Saját helyek lapon jön létre.</span><span class="sxs-lookup"><span data-stu-id="c3ec5-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="c3ec5-106">A jog megadásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="c3ec5-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="c3ec5-107">A SharePoint Felügyeleti központban kattintson a **felhasználói profilok**elemre.</span><span class="sxs-lookup"><span data-stu-id="c3ec5-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="c3ec5-108">A **Kapcsolatok** csoportban kattintson a **Felhasználói engedélyek kezelése gombra.**</span><span class="sxs-lookup"><span data-stu-id="c3ec5-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="c3ec5-109">Adjon hozzá olyan felhasználókat, akiknek engedélyre van szükségük a Saját helyek webhely létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="c3ec5-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="c3ec5-110">Alapértelmezés szerint ez a beállítás a **külső felhasználók kivételével mindenki**értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="c3ec5-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="c3ec5-111">Miután hozzáadta a felhasználót, felhasználókat vagy csoportot, győződjön meg arról, hogy a hozzáadott felhasználó, felhasználók vagy csoport ki van jelölve, görgessen az **engedélyek** szakaszhoz, majd jelölje be a **Személyes webhely létrehozása (személyes tároláshoz, hírcsatorna és követett tartalomhoz szükséges)** jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="c3ec5-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="c3ec5-112">Kattintson **az OK gombra,** majd keresse meg a felhasználót a OneDrive-lapon a webhely létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="c3ec5-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
