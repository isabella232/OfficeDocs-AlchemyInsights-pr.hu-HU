---
title: 646 hogyan kell beállítani a AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856658"
---
# <a name="configure-sync-features"></a><span data-ttu-id="33302-102">Szinkronizálási szolgáltatás konfigurálása</span><span class="sxs-lookup"><span data-stu-id="33302-102">Configure sync features</span></span>

<span data-ttu-id="33302-103">Azure AD csatlakozás tartalmaz számos szolgáltatása alapértelmezés szerint engedélyezve vannak, vagy később is engedélyezheti.</span><span class="sxs-lookup"><span data-stu-id="33302-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="33302-104">Egyes szolgáltatások igényel további konfigurálást adott környezetben.</span><span class="sxs-lookup"><span data-stu-id="33302-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="33302-105">Az objektumok [szűrése](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) korlátok Azure AD a rendszer szinkronizálja.</span><span class="sxs-lookup"><span data-stu-id="33302-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="33302-106">Alapértelmezés szerint minden felhasználók, kapcsolatok, csoportok, és a Windows 10 számítógépfiókot szinkronizálódnak.</span><span class="sxs-lookup"><span data-stu-id="33302-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="33302-107">Akkor figyelembe vehetjük vagy kihagyhatjuk objektumok tartományok, szervezeti egységek és más jellemzők alapján.</span><span class="sxs-lookup"><span data-stu-id="33302-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="33302-108">[Kivonat jelszó-szinkronizálás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) a jelszó kivonatértékét az Active Directory címtárból helyszíni Azure ad szinkronizálja.</span><span class="sxs-lookup"><span data-stu-id="33302-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="33302-109">Ez lehetővé teszi a jelszavak kezelését egy helyről, de ugyanazt a jelszót mindkét helyszíni és cloud környezetekben.</span><span class="sxs-lookup"><span data-stu-id="33302-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="33302-110">Mivel az Active Directory a mérvadó információforrás, használhatja a saját jelszóházirendek.</span><span class="sxs-lookup"><span data-stu-id="33302-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="33302-111">[Az önkiszolgáló jelszó alaphelyzetbe állítása (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) lehetővé teszi a felhasználók alaphelyzetbe saját jelszavukat a felhőben továbbra is az a helyi jelszóházirend alkalmazása közben.</span><span class="sxs-lookup"><span data-stu-id="33302-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="33302-112">[Eszköz visszaírása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) lehetővé teszi a regisztrált Azure Active Directory írják vissza a helyszíni Active Directory, a feltételes hozzáférésre használható.</span><span class="sxs-lookup"><span data-stu-id="33302-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="33302-113">[Véletlen rlés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) alapértelmezés szerint engedélyezve van túl sok egyidejű objektum törlése (500-nál több objektumot szinkronizálás) elkerülése érdekében.</span><span class="sxs-lookup"><span data-stu-id="33302-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="33302-114">Ez a beállítás a vállalata igényeinek megfelelően módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="33302-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="33302-115">Expressz telepítés esetén alapértelmezés szerint engedélyezett [az automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) , és így biztosítható a Azure AD csatlakozás verziója mindig aktuális.</span><span class="sxs-lookup"><span data-stu-id="33302-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
