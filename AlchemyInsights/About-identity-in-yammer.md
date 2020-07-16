---
title: Identitás a Yammerben
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
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148231"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="26630-102">Identitás a Yammerben</span><span class="sxs-lookup"><span data-stu-id="26630-102">About identity in Yammer</span></span>

<span data-ttu-id="26630-103">Javasoljuk, hogy minden hálózat tegye meg a következő lépéseket az identitással kapcsolatos problémák elkerülése érdekében:</span><span class="sxs-lookup"><span data-stu-id="26630-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="26630-104">Kényszerítse ki az Office 365-identitást, miután microsoft 365-fiókokat létesített az Azure AD felhasználói számára annak érdekében, hogy minden felhasználó az elsődleges Microsoft 365-fiókjával jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="26630-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="26630-105">További információ: [Office 365-identitás kényszerítése Yammer-felhasználók számára.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)</span><span class="sxs-lookup"><span data-stu-id="26630-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="26630-106">Több Yammer-hálózat konszolidálása.</span><span class="sxs-lookup"><span data-stu-id="26630-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="26630-107">Az örökölt Yammer-konfigurációk lehetővé teszik, hogy több Yammer-hálózat csatlakozzon egy bérlőhöz.</span><span class="sxs-lookup"><span data-stu-id="26630-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="26630-108">További információ: [Hálózati áttelepítés – Több Yammer-hálózat konszolidálása.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="26630-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="26630-109">Szükség esetén kényszerítheti a Yammer licencelését, hogy letiltsa a felhasználókat a Yammerből, ha nem rendelkeznek licenccel.</span><span class="sxs-lookup"><span data-stu-id="26630-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="26630-110">További információt a [Yammer-felhasználói licencek kezelése az Office 365-ben](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="26630-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="26630-111">Végül ellenőrizze a régebbi Yammer-hálózatok felhasználói listáját, és függessze fel az örökölt felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="26630-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="26630-112">Törlés helyett ajánlott felfüggeszteni (inaktiválni) a felhasználókat, mert a törlés visszafordíthatatlan.</span><span class="sxs-lookup"><span data-stu-id="26630-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="26630-113">További információt a [Yammer-felhasználók naplózása az Office 365-höz csatlakoztatott hálózatokban](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) és [a Felhasználók eltávolítása lapon](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)talál.</span><span class="sxs-lookup"><span data-stu-id="26630-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="26630-114">Ha ezekkel a lépésekkel konfigurálja a Yammert, akkor készen áll arra is, hogy a Yammer-hálózatot natív módra konfigurálja a Microsoft 365-höz.</span><span class="sxs-lookup"><span data-stu-id="26630-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="26630-115">További információt [a Yammer-hálózat konfigurálása natív módhoz a Microsoft 365 alkalmazáshoz című témakörben talál.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)</span><span class="sxs-lookup"><span data-stu-id="26630-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>