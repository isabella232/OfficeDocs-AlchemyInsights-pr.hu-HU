---
title: Fájlok megnyitása vagy letöltése a Yammerben
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
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148253"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="25c35-102">Fájlok megnyitása vagy letöltése a Yammerben</span><span class="sxs-lookup"><span data-stu-id="25c35-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="25c35-103">A klasszikus Yammer több lehetőséget is támogat az üzenetekbe és csoportokba való fájlfeltöltéshez.</span><span class="sxs-lookup"><span data-stu-id="25c35-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="25c35-104">A hálózati konfigurációtól függően a fájlok alapértelmezett tárolóhelyként szolgálnak a SharePointban.</span><span class="sxs-lookup"><span data-stu-id="25c35-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="25c35-105">Az új Yammer fájlválasztója még nem támogatja a klasszikus Yammerben elérhető összes lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="25c35-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="25c35-106">A jövőbeli frissítések további funkciókkal egészítik ki.</span><span class="sxs-lookup"><span data-stu-id="25c35-106">A future update will add additional features.</span></span> <span data-ttu-id="25c35-107">További információ: [Fájl vagy kép csatolása Yammer-beszélgetési bejegyzéshez című témakörben.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)</span><span class="sxs-lookup"><span data-stu-id="25c35-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="25c35-108">**Nem lehet megnyitni vagy letölteni egy fájlt**</span><span class="sxs-lookup"><span data-stu-id="25c35-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="25c35-109">Előfordulhat, hogy egy fájl feltöltésre kerül a Yammerbe, de a SharePoint Online-ban is hivatkozik egy fájlra.</span><span class="sxs-lookup"><span data-stu-id="25c35-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="25c35-110">A hibaelhárításhoz először meg kell határoznia a fájl helyét.</span><span class="sxs-lookup"><span data-stu-id="25c35-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="25c35-111">Ha a fájlt feltöltötték a Yammerbe, annak \*.yammer.com URL-címe lesz.</span><span class="sxs-lookup"><span data-stu-id="25c35-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="25c35-112">Győződjön meg arról, hogy a szükséges URL-címek és IP-címek le vannak tiltva.</span><span class="sxs-lookup"><span data-stu-id="25c35-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="25c35-113">További információt a [Yammer kemény kódolt IP-címeinek használata nem ajánlott](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)című blogbejegyzésben talál.</span><span class="sxs-lookup"><span data-stu-id="25c35-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="25c35-114">Ellenőrizze, hogy egy globális rendszergazdaként felhasználó letöltheti-e a fájlt.</span><span class="sxs-lookup"><span data-stu-id="25c35-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="25c35-115">Ha a fájl privát, előfordulhat, hogy privát tartalom módot kell használnia.</span><span class="sxs-lookup"><span data-stu-id="25c35-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="25c35-116">További információ: [Privát tartalmak figyelése a Yammerben.](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)</span><span class="sxs-lookup"><span data-stu-id="25c35-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="25c35-117">**A Yammer hálózati szintű vendégei és fájljai a SharePoint Online-ban**</span><span class="sxs-lookup"><span data-stu-id="25c35-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="25c35-118">[A Yammer hálózati szintű vendégei](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nem használják az Azure AD B2B-t, és a Yammer szolgáltatáson belül vannak, így nem férhetnek hozzá a SharePointban tárolt Yammer-fájlokhoz.</span><span class="sxs-lookup"><span data-stu-id="25c35-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="25c35-119">Hozzon létre egy külső AAD B2B-felhasználót, aki ezzel az identitással férhet hozzá a SharePoint Online-beli dokumentumtárakhoz.</span><span class="sxs-lookup"><span data-stu-id="25c35-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="25c35-120">Az Azure AD B2B jövőbeli vendégtámogatásáról a Yammerben a [Business-to-business (B2B) Vendégtámogatás a Yammer előzetes verziójában – Ügyfélfeltételek és gyakori kérdések című témakörben](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)talál további információt.</span><span class="sxs-lookup"><span data-stu-id="25c35-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>