---
title: KonzisztenciaGuid / sourceAnchor viselkedés
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705735"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="89063-102">KonzisztenciaGuid / sourceAnchor viselkedés</span><span class="sxs-lookup"><span data-stu-id="89063-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="89063-103">Az Azure AD Connect (1.1.524.0-s és újabb verzió) mostantól megkönnyíti az msDS-ConsistencyGuid sourceAnchor attribútumként való használatát.</span><span class="sxs-lookup"><span data-stu-id="89063-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="89063-104">A funkció használatakor az Azure AD Connect automatikusan konfigurálja a szinkronizálási szabályokat a következőkre:</span><span class="sxs-lookup"><span data-stu-id="89063-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="89063-105">Használja az msDS-ConsistencyGuid-ot a felhasználói objektumok sourceAnchor attribútumaként.</span><span class="sxs-lookup"><span data-stu-id="89063-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="89063-106">Az ObjectGUID más objektumtípusokhoz is használható.</span><span class="sxs-lookup"><span data-stu-id="89063-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="89063-107">Minden olyan helyszíni AD-felhasználó objektum, amelynek msDS-consistencyGuid attribútum nincs feltöltve, az Azure AD Connect írja az objectGUID értékét vissza az msDS-consistencyGuid attribútum a helyszíni Active Directoryban.</span><span class="sxs-lookup"><span data-stu-id="89063-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="89063-108">Az msDS-ConsistencyGuid attribútum feltöltése után az Azure AD Connect exportálja az objektumot az Azure AD-be.</span><span class="sxs-lookup"><span data-stu-id="89063-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="89063-109">**Megjegyzés:** Miután egy helyszíni AD-objektum ot importált az Azure AD Connect (azaz az AD-összekötő térbe importálva és a Metaverzumba vetítve), többé nem módosíthatja a sourceAnchor értékét.</span><span class="sxs-lookup"><span data-stu-id="89063-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="89063-110">Egy adott helyszíni AD-objektum sourceAnchor értékének megadásához konfigurálja az msDS-ConsistencyGuid attribútumot az Azure AD Connectbe történő importálás előtt.</span><span class="sxs-lookup"><span data-stu-id="89063-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="89063-111">A SourceAnchor és a ConsistencyGuid használatával kapcsolatos további információkért tekintse meg a következő t: [Azure AD Connect: Tervezési fogalmak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="89063-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

