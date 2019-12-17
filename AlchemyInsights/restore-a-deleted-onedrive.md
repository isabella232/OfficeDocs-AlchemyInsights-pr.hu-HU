---
title: Visszaállítani a törölt OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 5/15/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5298f192-326b-4820-b007-7e1a1c3c2b13
ms.openlocfilehash: a6db2e22c001cb809465c63da494121c06178b64
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054199"
---
# <a name="restore-a-deleted-onedrive"></a><span data-ttu-id="58187-102">Visszaállítani a törölt OneDrive</span><span class="sxs-lookup"><span data-stu-id="58187-102">Restore a deleted OneDrive</span></span>

<span data-ttu-id="58187-103">A felhasználó törlése után a felhasználó OneDrive-ja elérhető a Microsoft 365 Admin Center segítségével 30 napig.</span><span class="sxs-lookup"><span data-stu-id="58187-103">After you delete a user, you can access the user's OneDrive through the Microsoft 365 admin center for 30 days.</span></span> <span data-ttu-id="58187-104">Más felhasználók továbbra is hozzáférhetnek a megosztott tartalomhoz az OneDrive-ban, hogy mennyi ideig van beállítva az OneDrive admin központban.</span><span class="sxs-lookup"><span data-stu-id="58187-104">Other users can continue to access shared content in the OneDrive for the length of time you've set in the OneDrive admin center.</span></span> <span data-ttu-id="58187-105">(A beállítás módjáról [a törölt OneDrive felhasználók alapértelmezett fájlmegőrzési módjának beállítása](https://go.microsoft.com/fwlink/?linkid=874267)című témakörben olvashat.) Után amit idő, a OneDrive van mozgott-hoz újra feldolgoz tartó részére 93 napok, aztán-a ' töröl.</span><span class="sxs-lookup"><span data-stu-id="58187-105">(To learn how to set this, see [Set the default file retention for deleted OneDrive users](https://go.microsoft.com/fwlink/?linkid=874267).) After that time, the OneDrive is moved to the recycle bin for 93 days, and then it's deleted.</span></span>
  
<span data-ttu-id="58187-106">A kezdeti 30 nap után, amikor a törölt felhasználó már nem jelenik meg a Microsoft 365 Admin Center, elérheti a felhasználó OneDrive keresztül PowerShell.</span><span class="sxs-lookup"><span data-stu-id="58187-106">After the initial 30 days, when the deleted user no longer appears in the Microsoft 365 admin center, you can access the user's OneDrive through PowerShell.</span></span> <span data-ttu-id="58187-107">További információ: [a törölt OneDrive visszaállítása](https://go.microsoft.com/fwlink/?linkid=874269).</span><span class="sxs-lookup"><span data-stu-id="58187-107">For info, see [Restore a deleted OneDrive](https://go.microsoft.com/fwlink/?linkid=874269).</span></span>
  

