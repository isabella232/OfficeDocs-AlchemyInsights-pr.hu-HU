---
title: útmutató – nk2 kiterjesztésű-fájlok
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780061"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="d5594-102">A. nk2 kiterjesztésű fájlok importálása</span><span class="sxs-lookup"><span data-stu-id="d5594-102">How to import .nk2 files</span></span> 

<span data-ttu-id="d5594-103">Amikor első alkalommal elindítja a Microsoft Outlook 2013, az Outlook 2016, az Outlook 2019 vagy a Microsoft 365 Outlookot, a Felhasználónév gyorsítótára *(a nk2 kiterjesztésű*-fájlban tárolódik) az alapértelmezett üzenettároló alkalmazásban rejtett üzenetbe lesz importálva.</span><span class="sxs-lookup"><span data-stu-id="d5594-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="d5594-104">Ha a. nk2 kiterjesztésű fájlokat az Outlook 2013, az Outlook 2016, az Outlook 2019 vagy a Microsoft 365 Outlookba szeretné importálni, győződjön meg arról, hogy a. nk2 kiterjesztésű fájl a következő mappában található:%appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="d5594-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="d5594-105">**Megjegyzés**: a. nk2 kiterjesztésű fájlban a jelenlegi Outlook 2013-vagy Outlook 2016-profil nevének kell lennie.</span><span class="sxs-lookup"><span data-stu-id="d5594-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="d5594-106">A profilnév alapértelmezés szerint az "Outlook" nevet adja.</span><span class="sxs-lookup"><span data-stu-id="d5594-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="d5594-107">A profil nevének ellenőrzéséhez kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="d5594-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="d5594-108">Kattintson a **Start** menü **Vezérlőpult** parancsára.</span><span class="sxs-lookup"><span data-stu-id="d5594-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="d5594-109">Kattintson duplán a **posta**lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="d5594-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="d5594-110">A levelezési beállítások párbeszédpanelen válassza a **profilok megjelenítése**elemet.</span><span class="sxs-lookup"><span data-stu-id="d5594-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="d5594-111">Válassza **Start**a  >  **Futtatás**indítása gombot.</span><span class="sxs-lookup"><span data-stu-id="d5594-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="d5594-112">A **Megnyitás** mezőbe írja be a *outlook.exe/importnk2*, majd kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="d5594-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="d5594-113">Miután importálta a. nk2 kiterjesztésű fájlt, a fájl tartalma a postaládában tárolt meglévő becenév-gyorsítótárba kerül.</span><span class="sxs-lookup"><span data-stu-id="d5594-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="d5594-114">**Megjegyzés**: a. nk2 kiterjesztésű fájlt a. Old fájlnév-kiterjesztéssel nevezi át a következő alkalommal, amikor elindítja az Outlook 2013, az Outlook 2016, az Outlook 2019 vagy a Microsoft 365 Outlookot.</span><span class="sxs-lookup"><span data-stu-id="d5594-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="d5594-115">Ha újra importálni szeretné a. nk2 kiterjesztésű fájlt, először távolítsa el a. régi fájlnévkiterjesztéssel.</span><span class="sxs-lookup"><span data-stu-id="d5594-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="d5594-116">További információt [az automatikus kiegészítési lista importálása vagy másolása másik számítógépre](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="d5594-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>