---
title: MC210173 - SharePoint tervező új egyéni űrlaptulajdonság elavulása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928530"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="e7acf-102">MC210173 - SharePoint tervező új egyéni űrlaptulajdonság elavulása</span><span class="sxs-lookup"><span data-stu-id="e7acf-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="e7acf-103">Felfedeztünk egy olyan problémát, ami a SharePoint tervezőnek azt a funkcióját zavarja, ami az [egyéni űrlapokat hozza létre](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) a SharePoint online keretein belül.</span><span class="sxs-lookup"><span data-stu-id="e7acf-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="e7acf-104">Egy alapos vizsgálatot követően megállapítottuk, hogy erre a problémára nincs ismert megoldás, ezért úgy döntöttünk, hogy 2020. április 25-én szombaton, az egyezményes koordinált világidő szerint hajnali 3 órától letiltjuk az egyéni űrlaplétrehozás funkciót.</span><span class="sxs-lookup"><span data-stu-id="e7acf-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="e7acf-105">Ez a módosítás továbbra is engedi a korábban létrehozott űrlapok szerkesztését, és nem befolyásolja a SharePoint online tervező egyéb funkcióit.</span><span class="sxs-lookup"><span data-stu-id="e7acf-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="e7acf-106">A módosítást követően a felhasználók új űrlap létrehozása esetén a következő hibaüzenetet láthatják: „A lista változásai a szerverre nem menthetők”.</span><span class="sxs-lookup"><span data-stu-id="e7acf-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="e7acf-107">Azok a felhasználók, akik korábban a SharePoint tervezővel hoztak létre egyéni űrlapokat, a továbbiakban a [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) alkalmazást használhatják.</span><span class="sxs-lookup"><span data-stu-id="e7acf-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="e7acf-108">A PowerApps egy egyszerű és hatékony eszköz, amely lehetővé teszi, hogy a SharePoint online modern felületén működő felhasználók a SharePoint listák egyéni űrlapjait, illetve a dokumentumkönyvtárait közvetlenül a böngészőablakban hozzák létre, illetve szerkesszék.</span><span class="sxs-lookup"><span data-stu-id="e7acf-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="e7acf-109">A PowerApps nem igényel hagyományos kódolási ismereteket, illetve speciális alkalmazásletöltéseket, mint amilyen, például az InfoPath.</span><span class="sxs-lookup"><span data-stu-id="e7acf-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="e7acf-110">**Megjegyzés**: A SharePoint Online Classic felhasználók ideiglenesen kapcsoljanak át a Modern felületre, hogy hozzáférhessenek és használhassák a PowerApps alkalmazást, habár a PowerApps alkalmazásban létrehozott valamennyi egyéni űrlap elérhető a SharePoint Online Classic felület használói számára is.</span><span class="sxs-lookup"><span data-stu-id="e7acf-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
