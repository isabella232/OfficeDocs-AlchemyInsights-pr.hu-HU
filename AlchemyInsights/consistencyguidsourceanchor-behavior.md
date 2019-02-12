---
title: ConsistencyGuid / sourceAnchor viselkedés
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927653"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="e044d-102">ConsistencyGuid / sourceAnchor viselkedés</span><span class="sxs-lookup"><span data-stu-id="e044d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="e044d-p101">Azure AD csatlakozás (1.1.524.0 verzió, és utána) most lehetővé teszi az msDS-ConsistencyGuid sourceAnchor attribútum használatát. Ez a funkció használatakor Azure AD csatlakozás automatikusan beállítja a szinkronizálási szabályok:</span><span class="sxs-lookup"><span data-stu-id="e044d-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="e044d-p102">A sourceAnchor attribútum a felhasználói objektum msDS-ConsistencyGuid használják. ObjectGUID más objektumtípusok esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="e044d-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="e044d-p103">Bármely adott helyszíni AD felhasználói objektum, amelynek msDS-ConsistencyGuid attribútumot nem lakott, Azure AD csatlakozás írások az objectGUID értéket vissza a helyszíni Active Directory msDS-ConsistencyGuid attribútumot. Miután az msDS-ConsistencyGuid attribútumot nem üres, Azure AD csatlakozás majd exportálja az objektum Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e044d-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="e044d-p104">**Megjegyzés:** Egyszer helyszíni AD objektum Azure AD csatlakozás (azaz, importálja a összekötő AD helyet, és a Metaverse vetített) importálja, az sourceAnchor értékét már nem módosíthatja. Adhatja meg a sourceAnchor értékét egy adott helyszíni AD az objektum, az msDS-ConsistencyGuid attribútumot konfigurálása előtt Azure AD csatlakozás lesz importálva.</span><span class="sxs-lookup"><span data-stu-id="e044d-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="e044d-111">SourceAnchor és ConsistencyGuid további információt talál a következő: [Azure AD csatlakozás: tervezési koncepciók](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="e044d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

