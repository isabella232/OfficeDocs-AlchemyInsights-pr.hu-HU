---
title: ConsistencyGuid/sourceAnchor viselkedése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756285"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="9c2df-102">ConsistencyGuid/sourceAnchor viselkedése</span><span class="sxs-lookup"><span data-stu-id="9c2df-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="9c2df-103">Azure AD Connect (1.1.524.0-es verzió) most már megkönnyíti az msDS-ConsistencyGuid as sourceAnchor attribútum használatát.</span><span class="sxs-lookup"><span data-stu-id="9c2df-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="9c2df-104">A funkció használatakor az Azure AD Connect automatikusan beállítja a szinkronizálási szabályokat az alábbiak szerint:</span><span class="sxs-lookup"><span data-stu-id="9c2df-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="9c2df-105">Használja az msDS-ConsistencyGuid, mint a felhasználói objektumok sourceAnchor attribútumát.</span><span class="sxs-lookup"><span data-stu-id="9c2df-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="9c2df-106">A ObjectGUID más objektumtípusok számára van használatban.</span><span class="sxs-lookup"><span data-stu-id="9c2df-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="9c2df-107">Ha a helyszíni AD User objektumnak nincs kitöltve az msDS-ConsistencyGuid attribútuma, akkor az Azure AD Connect az objectGUID értékét visszaállítja a helyszíni Active Directory-beli msDS-ConsistencyGuid attribútumra.</span><span class="sxs-lookup"><span data-stu-id="9c2df-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="9c2df-108">Az msDS-ConsistencyGuid attribútum feltöltése után az Azure AD Connect ezt követően exportálja az objektumot az Azure AD-ra.</span><span class="sxs-lookup"><span data-stu-id="9c2df-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="9c2df-109">**Megjegyzés:** Ha a helyszíni AD-objektumot importálta az Azure AD Connectbe (azaz az AD Connector-területre importálja, és a metaverse-ba tervezi), már nem módosíthatja a sourceAnchor értékét.</span><span class="sxs-lookup"><span data-stu-id="9c2df-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="9c2df-110">Ha a helyszíni AD objektum sourceAnchor értékét szeretné megadni, akkor állítsa be az msDS-ConsistencyGuid attribútumot, mielőtt az Azure AD Connect programba importálja őket.</span><span class="sxs-lookup"><span data-stu-id="9c2df-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="9c2df-111">A SourceAnchor és a ConsistencyGuid további információt a következő témakörben találhat: [Azure ad Connect: tervezési fogalmak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="9c2df-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

