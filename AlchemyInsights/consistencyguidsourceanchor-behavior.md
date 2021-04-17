---
title: KonzisztenciaGuid/sourceAnchor behavior
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816994"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="6ca31-102">KonzisztenciaGuid/sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="6ca31-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="6ca31-103">Az Azure AD Connect (1.1.524.0-s és újabb verzió) mostantól megkönnyíti az msDS-ConsistencyGuid használatát sourceAnchor attribútumként.</span><span class="sxs-lookup"><span data-stu-id="6ca31-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="6ca31-104">A funkció használata esetén az Azure AD Connect automatikusan konfigurálja a szinkronizálási szabályokat a következő módon:</span><span class="sxs-lookup"><span data-stu-id="6ca31-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="6ca31-105">A user objektumok sourceAnchor attribútumaként használja az msDS-ConsistencyGuid attribútumot.</span><span class="sxs-lookup"><span data-stu-id="6ca31-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="6ca31-106">Az ObjectGUID más objektumtípusokhoz használatos.</span><span class="sxs-lookup"><span data-stu-id="6ca31-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="6ca31-107">Minden olyan helyszíni AD User objektum esetében, amelynek msDS-ConsistencyGuid attribútuma nincs feltöltve, az Azure AD Connect visszaírja az objektumGUID értékét az msDS-ConsistencyGuid attribútumba a helyszíni Active Directoryban.</span><span class="sxs-lookup"><span data-stu-id="6ca31-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="6ca31-108">Az msDS-ConsistencyGuid attribútum feltöltése után az Azure AD Connect ezután exportálja az objektumot az Azure AD szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="6ca31-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="6ca31-109">**Megjegyzés:** Miután egy helyszíni AD-objektumot importált az Azure AD Connect szolgáltatásba (amely az AD Connector Szóközbe importálva, majd a Metaverzába kivetítve történt), már nem módosíthatja a forrásAnchor értékét.</span><span class="sxs-lookup"><span data-stu-id="6ca31-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="6ca31-110">A sourceAnchor érték megadásához egy adott helyszíni AD-objektumhoz konfigurálja az msDS-ConsistencyGuid attribútumot az Azure AD Connectbe való importálás előtt.</span><span class="sxs-lookup"><span data-stu-id="6ca31-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="6ca31-111">További információ a SourceAnchor és a ConsistencyGuid szolgáltatásról: [Azure AD Connect:](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts) Tervezési fogalmak</span><span class="sxs-lookup"><span data-stu-id="6ca31-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

