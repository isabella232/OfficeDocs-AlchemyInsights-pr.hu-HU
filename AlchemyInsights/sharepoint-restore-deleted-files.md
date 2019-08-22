---
title: A törölt fájlok és mappák visszaállítása
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 604690e62f09b7ca0618c4a581605e22f19a7732
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507453"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="5c921-102">A törölt fájlok és mappák visszaállítása</span><span class="sxs-lookup"><span data-stu-id="5c921-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="5c921-103">SharePoint Online megtartja az összes tartalom biztonsági másolatait tényleges törlés 14 további napokhoz.</span><span class="sxs-lookup"><span data-stu-id="5c921-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="5c921-104">Tartalom a Lomtár vagy a fájlok visszaállítása nem állítható vissza, ha a rendszergazda a visszaállítás a 14 napos ablakon belül bármikor kérhet a Microsoft Support fordulhatnak segítségért.</span><span class="sxs-lookup"><span data-stu-id="5c921-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="5c921-105">A biztonsági másolat visszaállítását csak webhelycsoportok vagy alwebhely egyedi fájlok, listák vagy tárak esetében nem kell kitölteni.</span><span class="sxs-lookup"><span data-stu-id="5c921-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="5c921-106">Ha törlünk egy cikket vagy egy webhely Sharepoint-webhelyről, akkor nem azonnal eltávolítani.</span><span class="sxs-lookup"><span data-stu-id="5c921-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="5c921-107">A törölt elemek megnyitjuk a Lomtár egy ideig.</span><span class="sxs-lookup"><span data-stu-id="5c921-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="5c921-108">Ez idő alatt a törölt elemek visszaállíthatók eredeti helyükre.</span><span class="sxs-lookup"><span data-stu-id="5c921-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="5c921-109">További információért látogasson el az alábbi hivatkozásokra.</span><span class="sxs-lookup"><span data-stu-id="5c921-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="5c921-110">[Egy SharePoint-webhely a Lomtárban lévő elemek visszaállítása](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="5c921-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="5c921-111">Állítsa vissza a törölt fájlok és mappák OneDrive</span><span class="sxs-lookup"><span data-stu-id="5c921-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="5c921-112">Állítsa vissza a törölt webhelycsoport (beleértve a csoport, kommunikációs és egyéb helyek)</span><span class="sxs-lookup"><span data-stu-id="5c921-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="5c921-113">Törölt OneDrive a webhely visszaállítása</span><span class="sxs-lookup"><span data-stu-id="5c921-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="5c921-114">Tömeges újrahasznosítás bin műveletek rendszergazdák tekinthetik [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)segítségével.</span><span class="sxs-lookup"><span data-stu-id="5c921-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="5c921-115">**Fájlok visszaállítása szolgáltatás**</span><span class="sxs-lookup"><span data-stu-id="5c921-115">**Files Restore feature**</span></span>

<span data-ttu-id="5c921-116">Ha sok a OneDrive vagy a SharePoint-fájlok get törölt, felül, sérült vagy fertőzött malware, visszaállíthatja a teljes műsortárat OneDrive vagy a SharePoint egy korábbi időpontra, a fájlok visszaállítása szolgáltatással.</span><span class="sxs-lookup"><span data-stu-id="5c921-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="5c921-117">A OneDrive könyvtár visszaállítása</span><span class="sxs-lookup"><span data-stu-id="5c921-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="5c921-118">A dokumentumtár visszaállítása</span><span class="sxs-lookup"><span data-stu-id="5c921-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

