---
title: A OneDrive Vállalati webalkalmazás átirányítja a Delve-et
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799991"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="be0b2-102">Átirányítva a Delve-be, miután a OneDrive-ra kattintott</span><span class="sxs-lookup"><span data-stu-id="be0b2-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="be0b2-103">Tekintse meg részletes [hibaelhárítási útmutatónkat.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="be0b2-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="be0b2-104">A probléma megoldásához a rendszergazdának meg kell hoznia a felhasználóknak a saját webhelyek létrehozására vonatkozó jogot.</span><span class="sxs-lookup"><span data-stu-id="be0b2-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="be0b2-105">Ennek az az oka, hogy a OneDrive Vállalati verzió lap a Saját helyek lapon jön létre.</span><span class="sxs-lookup"><span data-stu-id="be0b2-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="be0b2-106">A jog megadásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="be0b2-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="be0b2-107">A SharePoint Felügyeleti központban kattintson a **felhasználói profilok elemre.**</span><span class="sxs-lookup"><span data-stu-id="be0b2-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="be0b2-108">A Személyek **csoportban** kattintson a **Felhasználói engedélyek kezelése elemre.**</span><span class="sxs-lookup"><span data-stu-id="be0b2-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="be0b2-109">Vegyen fel felhasználókat, akiknek engedélyre van szükségük a Saját helyek webhely létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="be0b2-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="be0b2-110">Ez a beállítás alapértelmezés szerint Mindenki, kivéve külső **felhasználók beállításra van állítva.**</span><span class="sxs-lookup"><span data-stu-id="be0b2-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="be0b2-111">Miután hozzáadta a felhasználót, felhasználókat vagy csoportot, győződjön meg arról, hogy a hozzáadott  felhasználó, felhasználók vagy csoport ki van jelölve, görgessen az Engedélyek szakaszhoz, és jelölje be a Személyes webhely létrehozása **(személyes tárhelyhez,** hírcsatornához és követett tartalomhoz szükséges) melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="be0b2-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="be0b2-112">Kattintson **az OK** gombra, majd a webhely létrehozásához keresse meg a OneDrive lapot.</span><span class="sxs-lookup"><span data-stu-id="be0b2-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
