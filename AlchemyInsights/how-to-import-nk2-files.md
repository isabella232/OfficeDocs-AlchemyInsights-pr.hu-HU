---
title: hogyan lehet importálni-nk2-fájlok
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759334"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="00a47-102">.nk2 fájlok importálása</span><span class="sxs-lookup"><span data-stu-id="00a47-102">How to import .nk2 files</span></span> 

<span data-ttu-id="00a47-103">Amikor először indítja el a Microsoft Outlook 2013, az Outlook 2016, az Outlook 2019 vagy a Microsoft 365 Outlook for Microsoft 365 programot, a becenév gyorsítótárát (a *profilnév*.nk2 fájlban tárolva) a rendszer rejtett üzenetbe importálja az alapértelmezett üzenettárolóban.</span><span class="sxs-lookup"><span data-stu-id="00a47-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="00a47-104">Ha .nk2 fájlt szeretne importálni az Outlook 2013,Outlook 2016, Outlook 2019 vagy Outlook for Microsoft 365 programba, győződjön meg arról, hogy az .nk2 fájl a következő mappában van: %appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="00a47-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="00a47-105">**Megjegyzés:** A .nk2 fájl nevének meg kell egyeznie a jelenlegi Outlook 2013- vagy Outlook 2016-profil nevével.</span><span class="sxs-lookup"><span data-stu-id="00a47-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="00a47-106">Alapértelmezés szerint a profil neve "Outlook".</span><span class="sxs-lookup"><span data-stu-id="00a47-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="00a47-107">A profil nevének ellenőrzéséhez kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="00a47-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="00a47-108">Kattintson **a Start**menü **Vezérlőpult parancsára.**</span><span class="sxs-lookup"><span data-stu-id="00a47-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="00a47-109">Kattintson duplán **a Posta**ikonra.</span><span class="sxs-lookup"><span data-stu-id="00a47-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="00a47-110">A Levelezés beállítása párbeszédpanelen válassza a **Profilok megjelenítése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="00a47-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="00a47-111">Válassza **a Futtatás indítása** > **Run**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="00a47-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="00a47-112">A **Megnyitás** mezőbe írja be az *outlook.exe /importnk2 parancsot,* majd kattintson **az OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="00a47-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="00a47-113">Az .nk2 fájl importálása után a fájl tartalma a postaládában tárolt meglévő becenév-gyorsítótárba kerül.</span><span class="sxs-lookup"><span data-stu-id="00a47-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="00a47-114">**Megjegyzés:** A .nk2 fájl .nk2 fájlja az Outlook 2013, az Outlook 2016, az Outlook 2019 vagy a Microsoft 365 Outlook for Outlook 365 következő indításakor .n2 fájlnévkiterjesztéssel lett átnevezve.</span><span class="sxs-lookup"><span data-stu-id="00a47-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="00a47-115">Ha újra importálni szeretné a .nk2 fájlt, először távolítsa el a .old fájlnévkiterjesztést.</span><span class="sxs-lookup"><span data-stu-id="00a47-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="00a47-116">További információt [az Automatikus kiegészítési lista importálása vagy másolása másik számítógépre](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="00a47-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>