---
title: a 646 beállítása a AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704491"
---
# <a name="configure-sync-features"></a><span data-ttu-id="70a65-102">Szinkronizálási szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="70a65-102">Configure sync features</span></span>

<span data-ttu-id="70a65-103">Az Azure AD Connect alapértelmezés szerint számos olyan funkciót tartalmaz, amely alapértelmezés szerint engedélyezve van, vagy később is engedélyezhető.</span><span class="sxs-lookup"><span data-stu-id="70a65-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="70a65-104">Egyes funkciókhoz további beállításokra van szükség bizonyos környezetekben.</span><span class="sxs-lookup"><span data-stu-id="70a65-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="70a65-105">[Szűrés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) : az objektumok szinkronizálása az Azure ad szolgáltatással történik.</span><span class="sxs-lookup"><span data-stu-id="70a65-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="70a65-106">Alapértelmezés szerint minden felhasználó, névjegy, csoport és Windows 10 számítógépfiók szinkronizálva van.</span><span class="sxs-lookup"><span data-stu-id="70a65-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="70a65-107">Az objektumokat tartományok, szervezeti egységek vagy egyéb attribútumok alapján is megadhatja vagy kihagyhatja.</span><span class="sxs-lookup"><span data-stu-id="70a65-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="70a65-108">A [jelszó-ujjlenyomat szinkronizálása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) szinkronizálja a jelszó-ujjlenyomatot a helyszíni Active Directoryból az Azure ad szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="70a65-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="70a65-109">Ez lehetővé teszi a jelszavak kezelését egyetlen helyen, de ugyanazt a jelszót használja mind a helyszíni, mind a Felhőbeli környezetekben.</span><span class="sxs-lookup"><span data-stu-id="70a65-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="70a65-110">Mivel az Active Directory a mérvadó forrás, használhatja saját jelszavas házirendjeit.</span><span class="sxs-lookup"><span data-stu-id="70a65-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="70a65-111">Önkiszolgáló [jelszó-visszaállító (Visszaállítás)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) : lehetővé teszi a felhasználóknak, hogy alaphelyzetbe állítsanak saját jelszavait a felhőben, miközben továbbra is alkalmazzák a helyszíni jelszavas házirendet.</span><span class="sxs-lookup"><span data-stu-id="70a65-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="70a65-112">Az [eszköz writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) lehetővé teszi, hogy az Azure ad-beli regisztrált eszközök visszalegyenek a helyszíni Active Directoryhoz, így felhasználhatók feltételes hozzáférésre.</span><span class="sxs-lookup"><span data-stu-id="70a65-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="70a65-113">A [véletlen törlések megelőzése](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) alapértelmezés szerint engedélyezve van, hogy ne legyenek túl sok egyidejű objektum törlése (több mint 500 objektum/szinkronizálás esetén).</span><span class="sxs-lookup"><span data-stu-id="70a65-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="70a65-114">Ezt a beállítást a szervezet igényeinek megfelelően változtathatja meg.</span><span class="sxs-lookup"><span data-stu-id="70a65-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="70a65-115">Az [automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) alapértelmezés szerint engedélyezve van az Express-telepítésekben, és biztosítja, hogy az Azure ad Connect verziója mindig naprakész legyen.</span><span class="sxs-lookup"><span data-stu-id="70a65-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
