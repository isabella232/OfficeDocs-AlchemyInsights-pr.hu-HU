---
title: Tartományszolgáltatás-szinkronizálás
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885155"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="f3981-102">Tartományszolgáltatás-szinkronizálás</span><span class="sxs-lookup"><span data-stu-id="f3981-102">Domain service synchronization</span></span>

<span data-ttu-id="f3981-103">Az Azure Active Directory tartományi szolgáltatások (Azure AD DS) felügyelt tartományában lévő objektumok és hitelesítő adatok vagy helyben, a tartományon belül, vagy egy Azure Active Directory (Azure AD) bérlői fiókból szinkronizálhatóak.</span><span class="sxs-lookup"><span data-stu-id="f3981-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="f3981-104">Amikor először telepíti az Azure AD DS-t, az Azure AD-ból replikálja az objektumokat egy automatikus, egy módon kezdeményezett szinkronizálás.</span><span class="sxs-lookup"><span data-stu-id="f3981-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="f3981-105">Ez az egy módszeres szinkronizálás továbbra is fut a háttérben, hogy az Azure AD DS felügyelt tartománya naprakész maradjon az Azure AD-ről származó esetleges módosításokkal.</span><span class="sxs-lookup"><span data-stu-id="f3981-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="f3981-106">Az Azure AD DS-ről nem történik újra szinkronizálás az Azure AD szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="f3981-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="f3981-107">Az Azure Active Directory tartományi szolgáltatások szinkronizálásával kapcsolatos további információkért lásd: [Tartományszolgáltatás-szinkronizálás.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)</span><span class="sxs-lookup"><span data-stu-id="f3981-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
