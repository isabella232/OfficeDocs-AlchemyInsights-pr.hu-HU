---
title: ConsistencyGuid/sourceAnchor viselkedés
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36516986"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="f7a29-102">ConsistencyGuid/sourceAnchor viselkedés</span><span class="sxs-lookup"><span data-stu-id="f7a29-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="f7a29-103">Azúrkék AD Connect (verzió 1.1.524.0 és utána) most megkönnyíti az msDS-ConsistencyGuid azonosító sourceAnchor attribútumként való használatát.</span><span class="sxs-lookup"><span data-stu-id="f7a29-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="f7a29-104">Ha ezt a funkciót használja, a Azure Connect program automatikusan beállítja a szinkronizálási szabályokat:</span><span class="sxs-lookup"><span data-stu-id="f7a29-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="f7a29-105">Használja a felhasználói objektumok sourceAnchor attribútumaként az msDS-ConsistencyGuid azonosítót.</span><span class="sxs-lookup"><span data-stu-id="f7a29-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="f7a29-106">Az ObjectGUID objektum más objektumtípusokhoz használatos.</span><span class="sxs-lookup"><span data-stu-id="f7a29-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="f7a29-107">Bármely olyan intézményi Active Directory felhasználói objektumhoz, amelynek msDS-ConsistencyGuid attribútuma nincs kitöltve, a Azure AD Connect az objectGUID értékét visszaírja az intézményi Active Directory msDS-ConsistencyGuid attribútumához.</span><span class="sxs-lookup"><span data-stu-id="f7a29-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="f7a29-108">Miután az msDS-ConsistencyGuid attribútum ki van töltve, a Azure AD Connect ezután exportálja az objektumot azúrkék AD-ba.</span><span class="sxs-lookup"><span data-stu-id="f7a29-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="f7a29-109">**Megjegyzés:** Miután egy intézményi Active Directory-objektumot importált a Azure AD Connect (azaz az AD Connector térbe, a metaverse értékre vetített) programba, már nem változtathatja meg a sourceAnchor értékét.</span><span class="sxs-lookup"><span data-stu-id="f7a29-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="f7a29-110">Egy adott intézményi Active Directory-objektumhoz tartozó sourceAnchor azonosító megadásához konfigurálja az msDS-ConsistencyGuid attribútumot az Azure AD Connect programba történő importálás előtt.</span><span class="sxs-lookup"><span data-stu-id="f7a29-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="f7a29-111">A SourceAnchor és a ConsistencyGuid azonosítóról további információt a következő címen olvashat: [Azure ad Connect: tervezési fogalmak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="f7a29-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

