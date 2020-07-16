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
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Fájlok megnyitása vagy letöltése a Yammerben

A klasszikus Yammer több lehetőséget is támogat az üzenetekbe és csoportokba való fájlfeltöltéshez. A hálózati konfigurációtól függően a fájlok alapértelmezett tárolóhelyként szolgálnak a SharePointban.

Az új Yammer fájlválasztója még nem támogatja a klasszikus Yammerben elérhető összes lehetőséget. A jövőbeli frissítések további funkciókkal egészítik ki. További információ: [Fájl vagy kép csatolása Yammer-beszélgetési bejegyzéshez című témakörben.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)

**Nem lehet megnyitni vagy letölteni egy fájlt**  

Előfordulhat, hogy egy fájl feltöltésre kerül a Yammerbe, de a SharePoint Online-ban is hivatkozik egy fájlra. A hibaelhárításhoz először meg kell határoznia a fájl helyét. Ha a fájlt feltöltötték a Yammerbe, annak *.yammer.com URL-címe lesz. Győződjön meg arról, hogy a szükséges URL-címek és IP-címek le vannak tiltva. További információt a [Yammer kemény kódolt IP-címeinek használata nem ajánlott](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)című blogbejegyzésben talál.

Ellenőrizze, hogy egy globális rendszergazdaként felhasználó letöltheti-e a fájlt. Ha a fájl privát, előfordulhat, hogy privát tartalom módot kell használnia. További információ: [Privát tartalmak figyelése a Yammerben.](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)  

**A Yammer hálózati szintű vendégei és fájljai a SharePoint Online-ban**  

[A Yammer hálózati szintű vendégei](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nem használják az Azure AD B2B-t, és a Yammer szolgáltatáson belül vannak, így nem férhetnek hozzá a SharePointban tárolt Yammer-fájlokhoz. Hozzon létre egy külső AAD B2B-felhasználót, aki ezzel az identitással férhet hozzá a SharePoint Online-beli dokumentumtárakhoz. Az Azure AD B2B jövőbeli vendégtámogatásáról a Yammerben a [Business-to-business (B2B) Vendégtámogatás a Yammer előzetes verziójában – Ügyfélfeltételek és gyakori kérdések című témakörben](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)talál további információt.