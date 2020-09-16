---
title: Tudnivalók az identitásról az Yammer-on
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664172"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="bc71c-102">Tudnivalók az identitásról az Yammer-on</span><span class="sxs-lookup"><span data-stu-id="bc71c-102">About identity in Yammer</span></span>

<span data-ttu-id="bc71c-103">Az identitással kapcsolatos problémák elkerülése érdekében ajánlott a minden hálózat a következő lépéseket végrehajtani:</span><span class="sxs-lookup"><span data-stu-id="bc71c-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="bc71c-104">Az Office 365-identitás érvényesítése a Microsoft 365-fiókok létesítése után az Azure AD felhasználói számára annak érdekében, hogy a felhasználók az elsődleges Microsoft 365-fiók segítségével bejelentkeznek.</span><span class="sxs-lookup"><span data-stu-id="bc71c-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="bc71c-105">További információt a Yammer- [felhasználók Office 365-identitásának érvényesítése](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="bc71c-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="bc71c-106">Több Yammer-hálózat összevonása.</span><span class="sxs-lookup"><span data-stu-id="bc71c-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="bc71c-107">A régebbi Yammer-konfigurációk lehetővé teszik, hogy több Yammer-hálózat csatlakozzon egy bérlőhöz.</span><span class="sxs-lookup"><span data-stu-id="bc71c-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="bc71c-108">További információt a [hálózati áttelepítés – több Yammer-hálózat megszilárdítása](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="bc71c-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="bc71c-109">Ha nem rendelkezik licenccel, akkor kényszerítheti a Yammer, hogy a felhasználók ne Yammer le a felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="bc71c-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="bc71c-110">További információt a [Yammer felhasználói licencek kezelése az Office 365-ban](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="bc71c-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="bc71c-111">Végezetül ellenőrizze a felhasználók listáját a régebbi Yammer-hálózatokhoz, és felfüggessze a régi felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="bc71c-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="bc71c-112">Javasoljuk, hogy a törlés helyett a felhasználókat felfüggessze (inaktiválja), mert a törlés visszafordíthatatlan.</span><span class="sxs-lookup"><span data-stu-id="bc71c-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="bc71c-113">További információt a [Yammer-felhasználók naplózása az Office 365-hoz csatlakoztatott hálózatokban](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) és a [felhasználók eltávolítása](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="bc71c-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="bc71c-114">Ha a fenti lépésekkel konfigurálja a Yammer, akkor is készen áll a Yammer-hálózat konfigurálására natív módra a Microsoft 365-ban.</span><span class="sxs-lookup"><span data-stu-id="bc71c-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="bc71c-115">További információt a Yammer- [hálózat beállítása natív módra a Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="bc71c-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>