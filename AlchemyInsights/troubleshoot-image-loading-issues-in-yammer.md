---
title: Képbetöltési problémák elhárítása a Yammerben
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148230"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="87166-102">Képbetöltési problémák elhárítása a Yammerben</span><span class="sxs-lookup"><span data-stu-id="87166-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="87166-103">Ha problémák merülnek fel a Yammerben lévő fényképekkel és fájlelőnézetekkel kapcsolatban, a probléma minden felhasználó számára jelentkezik-e, a mobileszközökön fordul-e elő, és a melléklet feltöltésekor reprodukálható-e.</span><span class="sxs-lookup"><span data-stu-id="87166-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="87166-104">**Profilfotózással kapcsolatos problémák**</span><span class="sxs-lookup"><span data-stu-id="87166-104">**Profile photo issues**</span></span>  

<span data-ttu-id="87166-105">Ha a végfelhasználók a Microsoft 365-ön keresztül jelentkeznek be a Yammerbe, meg kell változtatniuk a profiljukat, beleértve a profilképüket is.</span><span class="sxs-lookup"><span data-stu-id="87166-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="87166-106">Ha a felhasználók nem engedélyezték a profilfrissítéseket, a rendszergazda a felhasználó számára is elláthatja a frissítést.</span><span class="sxs-lookup"><span data-stu-id="87166-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="87166-107">További információt a [Profil megtekintése és frissítése az Office Delve-ben (View and update) témakörben talál.](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)</span><span class="sxs-lookup"><span data-stu-id="87166-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="87166-108">A profilszerkesztésről, beleértve a profilképeket is, a [Yammer-profil és a beállítások módosítása témakörben](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851)olvashat.</span><span class="sxs-lookup"><span data-stu-id="87166-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="87166-109">A frissített profilfotók szinkronizálása a profilattribútumoktól eltérően lesz.</span><span class="sxs-lookup"><span data-stu-id="87166-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="87166-110">A felhasználóknak be kell jelentkezniük, hogy kezdeményezzék a profilképük szinkronizálását.</span><span class="sxs-lookup"><span data-stu-id="87166-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="87166-111">További információt az [Office 365-ről a Yammerre frissített felhasználói profilképek](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)talál.</span><span class="sxs-lookup"><span data-stu-id="87166-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="87166-112">A Yammer felhasználói életciklusáról a [Yammer-felhasználók kezelése az Office 365-ből teljes életciklusuk során című témakörben talál.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)</span><span class="sxs-lookup"><span data-stu-id="87166-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="87166-113">A profilkép-szinkronizálás Microsoft 365-ben való [működéséről a Microsoft 365 profilkép-szinkronizálásáról szóló információ](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)című témakörben talál további információt.</span><span class="sxs-lookup"><span data-stu-id="87166-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="87166-114">**Dokumentumelőnézetekkel és képbélyegképpel kapcsolatos problémák**</span><span class="sxs-lookup"><span data-stu-id="87166-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="87166-115">Amikor fájlokat vagy képeket tesz közzé a Yammerben, előfordulhat, hogy az előnézetek nem jelennek meg a következők miatt:</span><span class="sxs-lookup"><span data-stu-id="87166-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="87166-116">A fájl sérült, ezért nem dolgozható fel.</span><span class="sxs-lookup"><span data-stu-id="87166-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="87166-117">A fájlt nem töltötte fel a közelmúltban a SharePoint Online-ba, vagy a Yammer más okok miatt érvénytelen metaadatokkal rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="87166-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="87166-118">Az előnézeti képek betöltéséhez szükséges URL-címek blokkolva vannak.</span><span class="sxs-lookup"><span data-stu-id="87166-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="87166-119">A fájl előnézetét a felhasználó a közzététel előtt eltávolította.</span><span class="sxs-lookup"><span data-stu-id="87166-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="87166-120">Egy szolgáltatásprobléma megakadályozta az előzetes verzió létrejöttét.</span><span class="sxs-lookup"><span data-stu-id="87166-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="87166-121">**Megjegyzés:** Előfordulhat, hogy a hivatkozások és a fájlfeltöltések előnézete eltérően viselkedik.</span><span class="sxs-lookup"><span data-stu-id="87166-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="87166-122">Előfordulhat, hogy az interneten található fájlokra vagy a további hitelesítést igénylő hivatkozásokra mutató hivatkozások nem jelennek meg megfelelően.</span><span class="sxs-lookup"><span data-stu-id="87166-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="87166-123">További információt a [Fájl vagy kép csatolása Yammer-üzenethez (Fájl vagy kép csatolása Yammer-üzenethez) témakörben talál.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)</span><span class="sxs-lookup"><span data-stu-id="87166-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 