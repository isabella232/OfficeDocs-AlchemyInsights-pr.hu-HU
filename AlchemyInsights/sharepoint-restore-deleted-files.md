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
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707524"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="361fb-102">Törölt fájl vagy mappa visszaállítása</span><span class="sxs-lookup"><span data-stu-id="361fb-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="361fb-103">A SharePoint Online megőrzi a teljes tartalom biztonsági mentését a tényleges törlést követő további 14 napig.</span><span class="sxs-lookup"><span data-stu-id="361fb-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="361fb-104">Ha a tartalom nem állítható vissza a Lomtár vagy a Fájl-visszaállítás segítségével, a rendszergazda kapcsolatba léphet a Microsoft ügyfélszolgálattal, és bármikor kérhet visszaállítást a 14 napos ablakon belül.</span><span class="sxs-lookup"><span data-stu-id="361fb-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="361fb-105">A biztonsági másolatokból történő visszaállítások csak a webhelycsoportok és az alwebhelyek esetén hajthatók végre, meghatározott fájlok, listák vagy tárak esetén nem.</span><span class="sxs-lookup"><span data-stu-id="361fb-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="361fb-106">Amikor töröl egy elemet vagy webhelyet a SharePointból, az nem törlődik azonnal.</span><span class="sxs-lookup"><span data-stu-id="361fb-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="361fb-107">A törölt elemek a Lomtárba kerülnek egy bizonyos ideig.</span><span class="sxs-lookup"><span data-stu-id="361fb-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="361fb-108">Ez alatt az idő alatt visszaállíthatja őket az eredeti helyükre.</span><span class="sxs-lookup"><span data-stu-id="361fb-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="361fb-109">További információkat az alábbi hivatkozásokon talál.</span><span class="sxs-lookup"><span data-stu-id="361fb-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="361fb-110">[SharePoint-webhely Lomtárában](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)lévő elemek visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="361fb-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="361fb-111">Törölt fájlok vagy mappák visszaállítása a OneDrive-ban</span><span class="sxs-lookup"><span data-stu-id="361fb-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="361fb-112">Törölt webhelycsoport visszaállítása (beleértve a csoportokat, a kommunikációt és más webhelyeket)</span><span class="sxs-lookup"><span data-stu-id="361fb-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="361fb-113">Törölt OneDrive-webhely visszaállítása</span><span class="sxs-lookup"><span data-stu-id="361fb-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="361fb-114">A tömeges lomtárműveletek esetén a rendszergazdák megfontolják a [SharePoint Online PNP-t.](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="361fb-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="361fb-115">**Fájlvisszaállítás funkció**</span><span class="sxs-lookup"><span data-stu-id="361fb-115">**Files Restore feature**</span></span>

<span data-ttu-id="361fb-116">Ha sok OneDrive- vagy SharePoint-fájlt törölnek, írnak felül, sérülnek meg vagy kártevők fertőzöttek, a fájl-visszaállítási funkcióval visszaállíthatja a teljes OneDrive- vagy SharePoint-tárat egy korábbi időpontra.</span><span class="sxs-lookup"><span data-stu-id="361fb-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="361fb-117">OneDrive-tárak visszaállítása</span><span class="sxs-lookup"><span data-stu-id="361fb-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="361fb-118">Dokumentumtárak visszaállítása</span><span class="sxs-lookup"><span data-stu-id="361fb-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

