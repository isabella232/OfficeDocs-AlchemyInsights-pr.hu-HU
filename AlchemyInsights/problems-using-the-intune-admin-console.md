---
title: Problémák az Intune felügyeleti konzoljának használatával
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555383"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="c4b3c-102">Problémák az Intune felügyeleti konzoljának használatával</span><span class="sxs-lookup"><span data-stu-id="c4b3c-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="c4b3c-103">**"Hozzáférés megtagadva" az Intune felügyeleti portálján való navigáláskor.**</span><span class="sxs-lookup"><span data-stu-id="c4b3c-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="c4b3c-104">Ha egy Intune-alapú egyéni szerepkör tagja, győződjön meg arról, hogy egy Intune-vagy Enterprise Mobility Suite (EMS) licenc van hozzárendelve a fiókjához.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="c4b3c-105">Ha a Configuration Manager segítségével kezeli az eszközöket, ellenőrizze, hogy nem tagja-e az Intune MDM-nek az Intune felhasználói gyűjteményében.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="c4b3c-106">Ellenőrizze, hogy rendelkezik-e a megfelelő szerepköralapú felügyeleti vezérlő (RBAC) engedélyekkel az Intune szerepkörök panelen.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="c4b3c-107">Ellenőrizze, hogy a használt csoport nem terjesztési lista-e.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="c4b3c-108">Az Intune az Azure Portalon csak az Azure Active Directory biztonsági csoportjaihoz tartozó felhasználói fiókokat támogatja.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="c4b3c-109">Tekintse át a csoportokat az Azure Portalon > **az Intune-csoportokban,**  >  **Groups**illetve az Azure Portalon > az Azure **Active Directoryban.**</span><span class="sxs-lookup"><span data-stu-id="c4b3c-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="c4b3c-110">**A felhasználó túl sok engedéllyel rendelkezik a hozzárendelt Intune-szerepkörhöz**</span><span class="sxs-lookup"><span data-stu-id="c4b3c-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="c4b3c-111">Azt tanácsolja a **Intune**felhasználónak, hogy lépjen az  >  **Intune-szerepkörök**saját  >  **engedélyek**  >  **rekettel** a megadott engedélyek áttekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="c4b3c-112">**Hozzáadtam egy hatókörcsoportot egy szerepkörhöz, de a szerepkörben lévő felhasználók továbbra is láthatják a többi felhasználót vagy eszközt.**</span><span class="sxs-lookup"><span data-stu-id="c4b3c-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="c4b3c-113">A hatókörcsoportok nem szűrik ki a felhasználókat vagy az eszközöket.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="c4b3c-114">Hatókörcsoportok:</span><span class="sxs-lookup"><span data-stu-id="c4b3c-114">Scope groups:</span></span>

- <span data-ttu-id="c4b3c-115">Korlátozhatja, hogy a felhasználók kihez rendelhetnek házirendeket vagy alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="c4b3c-116">Csak bizonyos felhasználók futtathatnak távoli feladatokat az eszközökön.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="c4b3c-117">A hatókörcsoportokról további információt a [Szerepköralapú hozzáférés-vezérlés (RBAC) és a Microsoft Intune (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="c4b3c-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="c4b3c-118">**Hozzáadtam egy felhasználót egy Intune-szerepkörhöz, de továbbra is teljes hozzáféréssel rendelkeznek az Intune felügyeleti konzoljához.**</span><span class="sxs-lookup"><span data-stu-id="c4b3c-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="c4b3c-119">Nyissa meg az Intune **>-felhasználók at** az Azure Portalon, és ellenőrizze, hogy a felhasználó nincs-e hozzárendelve az alábbi szerepkörök egyikéhez az Azure Portalon:</span><span class="sxs-lookup"><span data-stu-id="c4b3c-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="c4b3c-120">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="c4b3c-120">Global administrator</span></span>
- <span data-ttu-id="c4b3c-121">Az Intune szolgáltatás rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="c4b3c-121">Intune service administrator</span></span>
- <span data-ttu-id="c4b3c-122">SharePoint-rendszergazda</span><span class="sxs-lookup"><span data-stu-id="c4b3c-122">SharePoint administrator</span></span>

<span data-ttu-id="c4b3c-123">További információt a [Szerepköralapú hozzáférés-vezérlés (RBAC) és a Microsoft Intune című témakörben talál.](https://docs.microsoft.com/intune/role-based-access-control)</span><span class="sxs-lookup"><span data-stu-id="c4b3c-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="c4b3c-124">**Hozzáférési problémák**</span><span class="sxs-lookup"><span data-stu-id="c4b3c-124">**Access Issues**</span></span>

<span data-ttu-id="c4b3c-125">További információt az [Office 365-be, az Azure-ba vagy az Intune-ba való bejelentkezés nem tud bejelentkezni.](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)</span><span class="sxs-lookup"><span data-stu-id="c4b3c-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>