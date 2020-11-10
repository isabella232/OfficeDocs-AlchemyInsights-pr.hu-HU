---
title: OneDrive bejelentkezési hiba AADSTS50011
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
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982480"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="7cbc3-102">OneDrive bejelentkezési hiba AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="7cbc3-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="7cbc3-103">Ha hibaüzenet jelenik meg a "AADSTS50011: a kérésben megadott válasz URL-címe nem egyezik meg" üzenettel a OneDrive alkalmazásba való bejelentkezéskor, ellenőrizze az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="7cbc3-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="7cbc3-104">A OneDrive-verziónak a 20.052. XXXX verzióval egyenlőnek vagy nagyobbnak kell lennie. XXXX.</span><span class="sxs-lookup"><span data-stu-id="7cbc3-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="7cbc3-105">A verzió ellenőrzéséhez kattintson a kék OneDrive ikonra az értesítési területen, válassza a **súgó & a beállítások > a beállítások >** a beállítások lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7cbc3-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="7cbc3-106">A hálózat blokkolhatja a **g.Live.com** és a **oneclient.SFX.MS** való forgalmat.</span><span class="sxs-lookup"><span data-stu-id="7cbc3-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="7cbc3-107">Ha a forgalom le van tiltva, a OneDrive nem tudja frissíteni magát.</span><span class="sxs-lookup"><span data-stu-id="7cbc3-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="7cbc3-108">A hálózati rendszergazda segítségével gondoskodhat arról, hogy hozzáférhessen az URL-címekhez.</span><span class="sxs-lookup"><span data-stu-id="7cbc3-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="7cbc3-109">[Ezek a végpontok](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) elérhetők a Microsoft 365-csomagokat használó ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="7cbc3-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="7cbc3-110">Ha kézzel kell beszereznie a OneDrive aktuális verzióját, keresse fel [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="7cbc3-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
