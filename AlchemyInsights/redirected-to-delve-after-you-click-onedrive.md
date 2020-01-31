---
title: A OneDrive Vállalati web onedrive átirányítja a Delve-re
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
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571209"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="bbec5-102">Átirányítva a Delve-re, miután a OneDrive-ra kattintott</span><span class="sxs-lookup"><span data-stu-id="bbec5-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="bbec5-103">Tekintse meg részletes [hibaelhárítási útmutatónkat.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="bbec5-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="bbec5-104">A probléma megoldásához az Office 365 rendszergazdájának meg kell adnia a felhasználóknak a Saját helyek webhely létrehozásának jogát.</span><span class="sxs-lookup"><span data-stu-id="bbec5-104">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="bbec5-105">Ennek az az oka, hogy a OneDrive Vállalati verzió lap a Saját webhelyek lapon jön létre.</span><span class="sxs-lookup"><span data-stu-id="bbec5-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="bbec5-106">A jog megadásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="bbec5-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="bbec5-107">A SharePoint Felügyeleti központban kattintson a **felhasználói profilok**elemre.</span><span class="sxs-lookup"><span data-stu-id="bbec5-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="bbec5-108">A **Kapcsolatok** csoportban kattintson a **Felhasználói engedélyek kezelése**gombra.</span><span class="sxs-lookup"><span data-stu-id="bbec5-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="bbec5-109">Adjon hozzá olyan felhasználókat, akiknek engedélyre van szükségük a Saját helyek webhely létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="bbec5-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="bbec5-110">Alapértelmezés szerint ez a beállítás **a külső felhasználók kivételével mindenki**re van állítva.</span><span class="sxs-lookup"><span data-stu-id="bbec5-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="bbec5-111">Miután felvette a felhasználót, a felhasználókat vagy a csoportot, győződjön meg arról, hogy a hozzáadott felhasználó, felhasználók vagy csoportok be van jelölve, görgessen az **engedélyek** szakaszhoz, majd jelölje be a **Személyes webhely létrehozása (személyes tároláshoz, hírcsatorna és követett tartalomhoz szükséges)** jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="bbec5-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="bbec5-112">Kattintson az **OK**gombra, majd a webhely létrehozásához keresse meg a felhasználót a OneDrive lapon.</span><span class="sxs-lookup"><span data-stu-id="bbec5-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
