---
title: Fájlok elérése a Teams alkalmazásban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2675"
- "9000710"
ms.openlocfilehash: a00a39954737287b4888b833b66d98e9b5e711b2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668529"
---
# <a name="accessing-files-in-microsoft-teams"></a><span data-ttu-id="5e804-102">Fájlok elérése a Microsoft Teams alkalmazásban</span><span class="sxs-lookup"><span data-stu-id="5e804-102">Accessing files in Microsoft Teams</span></span>

<span data-ttu-id="5e804-103">Ha a felhasználók nehézségekbe ütköznek a Microsoft Teams-ban, először azt kell megállapítania, hogy a fájl privát csevegéshez vagy csatornás beszélgetéshez van csatolva.</span><span class="sxs-lookup"><span data-stu-id="5e804-103">If users have difficulty accessing a file in Microsoft Teams, first determine whether the file is attached to a private chat or a channel conversation.</span></span> <span data-ttu-id="5e804-104">A csapat csatornái olyan helyek, ahol a csoport minden tagja megnyithat egy beszélgetést.</span><span class="sxs-lookup"><span data-stu-id="5e804-104">Team channels are places where everyone on the team can openly have conversations.</span></span> <span data-ttu-id="5e804-105">A privát csevegések csak a csevegésben szereplő személyek számára láthatók (a csevegésben megosztott fájlok pedig a OneDrive vállalati verzióban vannak tárolva).</span><span class="sxs-lookup"><span data-stu-id="5e804-105">Private chats are only visible to those people in the chat (and files that you share in a chat are stored in OneDrive for Business).</span></span>

<span data-ttu-id="5e804-106">Ha a felhasználók privát csevegésben fájlokat osztanak meg, a fájl a megosztási felhasználó OneDrive vállalati verziójában tárolódik.</span><span class="sxs-lookup"><span data-stu-id="5e804-106">When users share files in private chats, the file is stored on the sharing user's OneDrive for Business.</span></span> <span data-ttu-id="5e804-107">Ha egy felhasználó hozzá lett adva egy meglévő privát csevegéshez, azok nem fognak tudni hozzáférni a fájlokhoz, kivéve ha az eredeti tulajdonos újra megosztja a fájlt.</span><span class="sxs-lookup"><span data-stu-id="5e804-107">If a user was added to an existing private chat, they won't be able to access the files unless the original owner re-shares the file.</span></span>    

<span data-ttu-id="5e804-108">**Csatornás beszélgetések esetén:**</span><span class="sxs-lookup"><span data-stu-id="5e804-108">**For channel conversations:**</span></span>

- <span data-ttu-id="5e804-109">A [Microsoft Teams fájljainak megosztása](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) a SharePointban vagy a OneDrive konfigurált beállításokon alapul.</span><span class="sxs-lookup"><span data-stu-id="5e804-109">[Sharing files in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) is based on the settings configured in SharePoint or OneDrive.</span></span> 
- <span data-ttu-id="5e804-110">Nézze át az [együttműködés a fájlokon csoporttal](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) című témakört, ahol többet is megtudhat arról, hogy a Teams hogyan teszi lehetővé szervezete számára a fájlok megosztását és együttműködését</span><span class="sxs-lookup"><span data-stu-id="5e804-110">Review [Collaborate on files with your Team](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) to learn more about how Teams allows your organization to share and collaborate on files.</span></span> 
- <span data-ttu-id="5e804-111">Ha az új csapattagok késésben vesznek részt a fájlok elérésében, várjon legalább **4 órát** , mielőtt megnyitná a támogatási jegyet a replikáció befejezésének engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="5e804-111">If new team members experience a delay in accessing files, please wait at least **4 hours** before opening a support ticket to allow replication to complete.</span></span> 

<span data-ttu-id="5e804-112">Ha a felhasználók korábban már hozzáfértek a fájlok a Teams-csatornán a fájlok lapon, és "ezek a fájlok már nem érhetők el" hibaüzenetet kaptak, ellenőrizze, hogy nem lett-e átnevezve a SharePoint-webhelyen vagy a dokumentumtárban.</span><span class="sxs-lookup"><span data-stu-id="5e804-112">If users could previously access files via the Files tab on a team channel, and you get a "these files are no longer available" error, check to see if the SharePoint site or document library has been renamed.</span></span> <span data-ttu-id="5e804-113">A SharePoint-webhelyek és a dokumentumtárak átnevezése még nem támogatott.</span><span class="sxs-lookup"><span data-stu-id="5e804-113">Renaming SharePoint sites and document libraries for Teams is not yet supported.</span></span> <span data-ttu-id="5e804-114">A probléma megoldásához nyissa meg a csoport számára használt csoportwebhely-webhelyet, és nevezze vissza a tárat a "megosztott dokumentumok" névre.</span><span class="sxs-lookup"><span data-stu-id="5e804-114">To resolve this issue, open the team site used for this team and rename the library back to “Shared Documents”.</span></span>