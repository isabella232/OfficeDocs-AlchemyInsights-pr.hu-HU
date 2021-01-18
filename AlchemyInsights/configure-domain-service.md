---
title: A tartományszolgáltatás konfigurálása
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885221"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="29d1a-102">Nem lehet engedélyezni az AAD-DS-t, vagy a telepítés nem működik</span><span class="sxs-lookup"><span data-stu-id="29d1a-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="29d1a-103">Az Azure AD tartományszolgáltatás (AAD-DS) nem engedélyezett vagy telepítésének sikertelen voltát az alábbi lépésekkel oldhatja meg:</span><span class="sxs-lookup"><span data-stu-id="29d1a-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="29d1a-104">Ha már meglévő virtuális hálózatot használ, ellenőrizze, hogy a NSG-ben nincsenek-e olyan szabályok, amelyek letiltják a portál AAD-DS szolgáltatásában való szinkronizáláshoz szükséges https://aka.ms/aadds-networking portokat.</span><span class="sxs-lookup"><span data-stu-id="29d1a-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="29d1a-105">Ellenőrizze, hogy a hibaüzenetre választ talált-e ebben a hibaelhárítási útmutatóban, amely elérhető ebben a  https://aka.ms/aadds-troubleshoot-enable témakörben.</span><span class="sxs-lookup"><span data-stu-id="29d1a-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="29d1a-106">Próbálja meg telepíteni az Azure AD Domain Services szolgáltatást egy új virtuális hálózaton.</span><span class="sxs-lookup"><span data-stu-id="29d1a-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="29d1a-107">Kövesse az Első lépések útmutatót az AAD-DS telepítéséhez: Az AAD tartományi szolgáltatások [létrehozása és konfigurálása.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)</span><span class="sxs-lookup"><span data-stu-id="29d1a-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="29d1a-108">Ha problémákat ad az Azure AD domain Services üzembe helyezésével kapcsolatban, az [Azure AD tartományi](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) szolgáltatások hibaelhárításával kapcsolatos témakörben kijavíthatja a gyakori hibákat, amelyek segíthetnek az újra működő szolgáltatások használatában.</span><span class="sxs-lookup"><span data-stu-id="29d1a-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="29d1a-109">**Nem lehet letiltani az AAD-DS-t**</span><span class="sxs-lookup"><span data-stu-id="29d1a-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="29d1a-110">Az AAD-DS nem szüneteltetheti a lejátszást.</span><span class="sxs-lookup"><span data-stu-id="29d1a-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="29d1a-111">Ha nem szeretné tovább használni a felügyelt tartományt, törölnie kell azt.</span><span class="sxs-lookup"><span data-stu-id="29d1a-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="29d1a-112">A felügyelt tartomány törléséről az [AAD-tartományszolgáltatás törlése csoportban található.](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)</span><span class="sxs-lookup"><span data-stu-id="29d1a-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



