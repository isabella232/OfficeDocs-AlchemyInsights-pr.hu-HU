---
title: Jelszó kivonatszinkronizálása a tartományszolgáltatáshoz
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177489"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="1c361-102">Jelszó kivonatszinkronizálása a tartományszolgáltatáshoz</span><span class="sxs-lookup"><span data-stu-id="1c361-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="1c361-103">**Ha az Azure AD DS-példánya jelszó-kivonat-szinkronizálás engedélyezését kéri**</span><span class="sxs-lookup"><span data-stu-id="1c361-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="1c361-104">Olyan helyzettel találkozhat, amelyben hibrid környezetet futtat, amelyben a felhasználók helyszíni Azure Active Directory tartományi szolgáltatások (AD DS) környezetből szinkronizálnak.</span><span class="sxs-lookup"><span data-stu-id="1c361-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="1c361-105">Ez a helyzet annak ellenére merül fel, hogy jelszó-kivonat-szinkronizálást használ a helyszíni AD DS-ről az Azure AD-bérlőjébe.</span><span class="sxs-lookup"><span data-stu-id="1c361-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="1c361-106">**A probléma oka**</span><span class="sxs-lookup"><span data-stu-id="1c361-106">**Cause**</span></span>

<span data-ttu-id="1c361-107">Ennek az az oka, hogy az Azure AD Connect alapértelmezés szerint nem szinkronizálja az Azure AD DS-hez szükséges régi New Technology LAN Manager -előfizetéseket és Kerberos-jelszavakat.</span><span class="sxs-lookup"><span data-stu-id="1c361-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="1c361-108">**Kerülő megoldás**</span><span class="sxs-lookup"><span data-stu-id="1c361-108">**Workaround**</span></span> 

<span data-ttu-id="1c361-109">Konfigurálnia kell az Azure AD Connectet az NTLM- és Kerberos-hitelesítéshez szükséges jelszó-előjelszavak szinkronizálásához.</span><span class="sxs-lookup"><span data-stu-id="1c361-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="1c361-110">Miután konfigurálta az Azure AD Connectet, egy helyszíni fiók létrehozása vagy jelszó-módosítási esemény is szinkronizálja a régi jelszó-előjeleket az Azure AD-be.</span><span class="sxs-lookup"><span data-stu-id="1c361-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="1c361-111">Erről [és](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) arról, hogy miként engedélyezheti a jelszó-szinkronizálást az Azure AD DS hibrid környezetében, olvassa el itt a további információkat.</span><span class="sxs-lookup"><span data-stu-id="1c361-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>