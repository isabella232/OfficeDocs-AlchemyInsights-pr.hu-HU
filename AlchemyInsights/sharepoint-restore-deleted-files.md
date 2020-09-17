---
title: Törölt fájl vagy mappa visszaállítása
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797550"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="8ba45-102">Törölt fájl vagy mappa visszaállítása</span><span class="sxs-lookup"><span data-stu-id="8ba45-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="8ba45-103">A SharePoint Online megőrzi a teljes tartalom biztonsági mentését a tényleges törlést követő további 14 napig.</span><span class="sxs-lookup"><span data-stu-id="8ba45-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="8ba45-104">Ha a Lomtárban vagy a fájlok visszaállításakor nem lehet visszaállítani a tartalmat, a rendszergazda felhívhatja a Microsoft támogatási szolgálatát, hogy a 14 napos ablakon belül bármikor vissza lehessen állítani a visszaállítást.</span><span class="sxs-lookup"><span data-stu-id="8ba45-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="8ba45-105">A biztonsági másolatokból történő visszaállítások csak a webhelycsoportok és az alwebhelyek esetén hajthatók végre, meghatározott fájlok, listák vagy tárak esetén nem.</span><span class="sxs-lookup"><span data-stu-id="8ba45-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="8ba45-106">Ha töröl egy elemet vagy webhelyet a Sharepointból, az nem törlődik azonnal.</span><span class="sxs-lookup"><span data-stu-id="8ba45-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="8ba45-107">A törölt elemek a Lomtárba kerülnek egy bizonyos ideig.</span><span class="sxs-lookup"><span data-stu-id="8ba45-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="8ba45-108">Ez alatt az idő alatt visszaállíthatja őket az eredeti helyükre.</span><span class="sxs-lookup"><span data-stu-id="8ba45-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="8ba45-109">További információkat az alábbi hivatkozásokon talál.</span><span class="sxs-lookup"><span data-stu-id="8ba45-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="8ba45-110">[SharePoint-webhely Lomtárában lévő elemek visszaállítása](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)</span><span class="sxs-lookup"><span data-stu-id="8ba45-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="8ba45-111">Törölt fájlok vagy mappák visszaállítása a OneDrive-ban</span><span class="sxs-lookup"><span data-stu-id="8ba45-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="8ba45-112">Törölt webhelycsoport visszaállítása (többek között a csoporttal, a kommunikációval és más webhelyekkel)</span><span class="sxs-lookup"><span data-stu-id="8ba45-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="8ba45-113">Törölt OneDrive-webhely visszaállítása</span><span class="sxs-lookup"><span data-stu-id="8ba45-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="8ba45-114">A tömeges Lomtár-műveletek esetében a rendszergazdák a [SharePoint Online PnP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)használatát is fontolóra vehetik.</span><span class="sxs-lookup"><span data-stu-id="8ba45-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="8ba45-115">**Fájlvisszaállítás funkció**</span><span class="sxs-lookup"><span data-stu-id="8ba45-115">**Files Restore feature**</span></span>

<span data-ttu-id="8ba45-116">Ha a OneDrive-vagy SharePoint-fájljait a program törli, felülírja, elrontotta vagy fertőzte meg, a fájlok visszaállítása funkció segítségével visszaállíthatja a teljes OneDrive vagy a SharePoint-tárat.</span><span class="sxs-lookup"><span data-stu-id="8ba45-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="8ba45-117">OneDrive-tárak visszaállítása</span><span class="sxs-lookup"><span data-stu-id="8ba45-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="8ba45-118">Dokumentumtárak visszaállítása</span><span class="sxs-lookup"><span data-stu-id="8ba45-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

