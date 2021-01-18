---
title: Probléma a virtuális gépekhez való csatlakozásnál
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885209"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="db908-102">Probléma a virtuális gépekhez való csatlakozásnál</span><span class="sxs-lookup"><span data-stu-id="db908-102">Issue joining VMs</span></span>

<span data-ttu-id="db908-103">A következő lépésekkel oldhatja meg a virtuális gépekhez való csatlakozáskor előforduló problémákat:</span><span class="sxs-lookup"><span data-stu-id="db908-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="db908-104">Próbáljon meg **upn** formátumban (például "joeuser@contoso.com") bejelentkezni a **SAMAccountName** formátum ('CONTOSO\jojauser') helyett.</span><span class="sxs-lookup"><span data-stu-id="db908-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="db908-105">Győződjön meg arról, hogy az első lépéseket  követve engedélyezte a jelszó-szinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="db908-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="db908-106">Győződjön meg arról, hogy az érintett felhasználói fiók nem külső fiók az Azure AD bérlői webhelyen.</span><span class="sxs-lookup"><span data-stu-id="db908-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="db908-107">A külső felhasználók nem tudnak bejelentkezni a felügyelt tartományba, mert az Azure AD tartományi szolgáltatások nem tartalmaznak hitelesítő adatokat az ilyen felhasználói fiókokhoz.</span><span class="sxs-lookup"><span data-stu-id="db908-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="db908-108">Ha az érintett felhasználói fiók csak felhőalapú felhasználói fiók, győződjön meg arról, hogy a felhasználók megváltoztatták a jelszavukat az Azure AD tartományi szolgáltatások engedélyezése után.</span><span class="sxs-lookup"><span data-stu-id="db908-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="db908-109">Ez a lépés az Azure AD tartományi szolgáltatások generálása érdekében szükséges hitelesítő adatokhoz szükséges hitelesítő adatokat generálja.</span><span class="sxs-lookup"><span data-stu-id="db908-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="db908-110">Ha az érintett felhasználói fiókok szinkronizálva vannak egy helyszíni címtárból, ellenőrizze, hogy az Azure AD Connect ajánlott kiadása be van-e állítva teljes szinkronizálásra.</span><span class="sxs-lookup"><span data-stu-id="db908-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="db908-111">Ha a 4. lépés megerősítése után a problémák továbbra is fennállnak, hajtsa végre a következő parancsokat a szinkronizálási gépről:</span><span class="sxs-lookup"><span data-stu-id="db908-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="db908-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="db908-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>