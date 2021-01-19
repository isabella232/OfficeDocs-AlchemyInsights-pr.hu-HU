---
title: Tartományvezérlő
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901025"
---
# <a name="domain-controller"></a><span data-ttu-id="4c35e-102">Tartományvezérlő</span><span class="sxs-lookup"><span data-stu-id="4c35e-102">Domain controller</span></span>

<span data-ttu-id="4c35e-103">**Nem lehet engedélyezni az AAD-DS-t, vagy a telepítés nem működik**</span><span class="sxs-lookup"><span data-stu-id="4c35e-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="4c35e-104">Az Azure AD tartományszolgáltatás (AAD-DS) nem engedélyezett vagy telepítésének sikertelen voltát az alábbi lépésekkel oldhatja meg:</span><span class="sxs-lookup"><span data-stu-id="4c35e-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="4c35e-105">Ha már meglévő virtuális hálózatot használ, ellenőrizze, hogy a NSG-ben nincsenek-e olyan szabályok, amelyek letiltják a portál AAD-DS szolgáltatásában való szinkronizáláshoz szükséges https://aka.ms/aadds-networking portokat.</span><span class="sxs-lookup"><span data-stu-id="4c35e-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="4c35e-106">Ellenőrizze, hogy a hibaüzenetre választ talált-e ebben a hibaelhárítási útmutatóban, amely elérhető ebben a  https://aka.ms/aadds-troubleshoot-enable témakörben.</span><span class="sxs-lookup"><span data-stu-id="4c35e-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="4c35e-107">Próbálja meg telepíteni az Azure AD Domain Services szolgáltatást egy új virtuális hálózaton.</span><span class="sxs-lookup"><span data-stu-id="4c35e-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="4c35e-108">Kövesse az Első lépések útmutatót az AAD-DS telepítéséhez, amely az Azure AD tartományi szolgáltatások létrehozásáról [oktatóprogramban érhető el.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)</span><span class="sxs-lookup"><span data-stu-id="4c35e-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="4c35e-109">Ha problémákat ad az Azure AD domain Services üzembe helyezésével kapcsolatban, az [Azure AD tartományi](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) szolgáltatások hibaelhárításával kapcsolatos témakörben kijavíthatja a gyakori hibákat, amelyek segíthetnek az újra működő szolgáltatások használatában.</span><span class="sxs-lookup"><span data-stu-id="4c35e-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="4c35e-110">**Nem lehet letiltani az AAD-DS-t**</span><span class="sxs-lookup"><span data-stu-id="4c35e-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="4c35e-111">Az AAD-DS nem szüneteltetheti a lejátszást.</span><span class="sxs-lookup"><span data-stu-id="4c35e-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="4c35e-112">Ha nem szeretné tovább használni a felügyelt tartományt, törölnie kell azt.</span><span class="sxs-lookup"><span data-stu-id="4c35e-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="4c35e-113">Ha problémák lépnek fel, a gyakori hibaüzenetek megoldásához és a kapcsolódó hibaelhárítási lépésekhez, amelyek segítenek az újrafuttatásban, tekintse át az Azure Active Directory tartományi szolgáltatások [hibaelhárítási lépéseit.](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="4c35e-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
