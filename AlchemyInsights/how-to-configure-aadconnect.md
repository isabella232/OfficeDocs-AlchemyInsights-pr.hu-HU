---
title: 646 Az AADConnect konfigurálása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722561"
---
# <a name="configure-sync-features"></a><span data-ttu-id="29fda-102">Szinkronizálási szolgáltatások konfigurálása</span><span class="sxs-lookup"><span data-stu-id="29fda-102">Configure sync features</span></span>

<span data-ttu-id="29fda-103">Az Azure AD Connect számos olyan funkciót tartalmaz, amelyek alapértelmezés szerint engedélyezve vannak, vagy amelyeket később engedélyezhet.</span><span class="sxs-lookup"><span data-stu-id="29fda-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="29fda-104">Egyes szolgáltatások további konfigurációt igényelnek bizonyos környezetekben.</span><span class="sxs-lookup"><span data-stu-id="29fda-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="29fda-105">[A szűrés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) korlátozza az objektumok szinkronizálását az Azure AD-vel.</span><span class="sxs-lookup"><span data-stu-id="29fda-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="29fda-106">Alapértelmezés szerint a rendszer minden felhasználót, kapcsolattartót, csoportot és Windows 10-es számítógépfiókot szinkronizál.</span><span class="sxs-lookup"><span data-stu-id="29fda-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="29fda-107">Tartományon, ous-okon vagy más attribútumokon alapuló objektumokat is felvehet vagy kizárhat.</span><span class="sxs-lookup"><span data-stu-id="29fda-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="29fda-108">[A jelszókivonat-szinkronizálás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) szinkronizálja a jelszókivonatot a helyszíni Active Directoryból az Azure AD-be.</span><span class="sxs-lookup"><span data-stu-id="29fda-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="29fda-109">Ez lehetővé teszi a jelszókezelést egy helyen, de ugyanazt a jelszót használja mind a helyszíni, mind a felhőalapú környezetekben.</span><span class="sxs-lookup"><span data-stu-id="29fda-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="29fda-110">Mivel az Active Directory a mérvadó forrás, használhatja a saját jelszóházirendeket.</span><span class="sxs-lookup"><span data-stu-id="29fda-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="29fda-111">[Az önkiszolgáló jelszó-visszaállítás (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) lehetővé teszi a felhasználók számára, hogy alaphelyzetbe állítsák saját jelszavukat a felhőben, miközben továbbra is alkalmazzák a helyszíni jelszóházirendet.</span><span class="sxs-lookup"><span data-stu-id="29fda-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="29fda-112">[Az eszközvisszaírás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) lehetővé teszi, hogy az Azure AD-ben regisztrált eszközök visszaírhatók legyenek a helyszíni Active Directoryba, így feltételes hozzáféréshez használhatók.</span><span class="sxs-lookup"><span data-stu-id="29fda-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="29fda-113">[A véletlen törlés megakadályozása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) alapértelmezés szerint engedélyezve van a túl sok egyidejű objektumtörlés megakadályozása érdekében (szinkronizálásonként több mint 500 objektum).</span><span class="sxs-lookup"><span data-stu-id="29fda-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="29fda-114">Ezt a beállítást a szervezet igényeinek megfelelően módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="29fda-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="29fda-115">[Az automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) alapértelmezés szerint engedélyezve van az expressz telepítésekhez, és biztosítja, hogy az Azure AD Connect verziója mindig aktuális legyen.</span><span class="sxs-lookup"><span data-stu-id="29fda-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
