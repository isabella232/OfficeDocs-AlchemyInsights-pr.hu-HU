---
title: Törölt fájl vagy mappa visszaállítása
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 2702837bff2c0a465dde2c090a44e02747cc85ec
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051067"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="9ac0e-102">Törölt fájl vagy mappa visszaállítása</span><span class="sxs-lookup"><span data-stu-id="9ac0e-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="9ac0e-103">A SharePoint Online a tényleges törlést követő 14 további napra megőrzi az összes tartalom biztonsági másolatait.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="9ac0e-104">Ha a tartalom nem állítható vissza a Lomtár vagy a fájlok visszaállítása segítségével, a rendszergazda a Microsoft terméktámogatási webhelyére bármikor helyreállíthat egy visszaállítási kérelmet a 14 napos ablakban.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="9ac0e-105">A biztonsági másolatokból történő visszaállítások csak webhelycsoportok vagy alwebhelyek esetén fejezhetők be, meghatározott fájlokhoz, listákhoz vagy tárakhoz nem.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="9ac0e-106">Ha töröl egy elemet vagy webhelyet a SharePoint alkalmazásból, az nem törlődik azonnal.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="9ac0e-107">A törölt elemek egy ideig a Lomtárba kerülnek.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="9ac0e-108">Ez alatt az idő alatt visszaállíthatjuk az eredeti helyére törölt elemeket.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="9ac0e-109">További információért kérjük, látogasson el az alábbi linkekre.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="9ac0e-110">[Egy SharePoint-webhely Lomtárában lévő elemek visszaállítása](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="9ac0e-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="9ac0e-111">Visszaad töröl fájlokat vagy tartók-ban OneDrive</span><span class="sxs-lookup"><span data-stu-id="9ac0e-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="9ac0e-112">Törölt webhelycsoport visszaállítása (beleértve a csoportot, a kommunikációt és más webhelyeket)</span><span class="sxs-lookup"><span data-stu-id="9ac0e-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="9ac0e-113">A törölt OneDrive webhely visszaállítása</span><span class="sxs-lookup"><span data-stu-id="9ac0e-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="9ac0e-114">A tömeges Lomtár-műveletek esetében az adminisztrátorok megfontolhatják a [SharePoint Online PnP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)használatát.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="9ac0e-115">**Fájlok visszaállítása szolgáltatás**</span><span class="sxs-lookup"><span data-stu-id="9ac0e-115">**Files Restore feature**</span></span>

<span data-ttu-id="9ac0e-116">Ha egy halom-a OneDrive vagy SharePoint fájlokat kap töröl, átírt, elrontott, vagy fertőzött mellett malware, tudod visszaad-a teljes OneDrive vagy SharePoint könyvtár-hoz egy előző idő használ a fájlokat visszaad vonás.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="9ac0e-117">OneDrive függvénytár visszaállítása</span><span class="sxs-lookup"><span data-stu-id="9ac0e-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="9ac0e-118">Dokumentumtár visszaállítása</span><span class="sxs-lookup"><span data-stu-id="9ac0e-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

