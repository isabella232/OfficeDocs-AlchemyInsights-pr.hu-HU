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
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408110"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="38edc-102">ConsistencyGuid / sourceAnchor viselkedés</span><span class="sxs-lookup"><span data-stu-id="38edc-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="38edc-103">Azure AD csatlakozás (1.1.524.0 verzió, és utána) most lehetővé teszi az msDS-ConsistencyGuid sourceAnchor attribútum használatát.</span><span class="sxs-lookup"><span data-stu-id="38edc-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="38edc-104">Ez a funkció használatakor Azure AD csatlakozás automatikusan beállítja a szinkronizálási szabályok:</span><span class="sxs-lookup"><span data-stu-id="38edc-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="38edc-105">A sourceAnchor attribútum a felhasználói objektum msDS-ConsistencyGuid használják.</span><span class="sxs-lookup"><span data-stu-id="38edc-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="38edc-106">ObjectGUID más objektumtípusok esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="38edc-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="38edc-107">Bármely adott helyszíni AD felhasználói objektum, amelynek msDS-ConsistencyGuid attribútumot nem lakott, Azure AD csatlakozás írások az objectGUID értéket vissza a helyszíni Active Directory msDS-ConsistencyGuid attribútumot.</span><span class="sxs-lookup"><span data-stu-id="38edc-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="38edc-108">Miután az msDS-ConsistencyGuid attribútumot nem üres, Azure AD csatlakozás majd exportálja az objektum Azure AD.</span><span class="sxs-lookup"><span data-stu-id="38edc-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="38edc-109">**Megjegyzés:** Egyszer helyszíni AD objektum Azure AD csatlakozás (azaz, importálja a összekötő AD helyet, és a Metaverse vetített) importálja, az sourceAnchor értékét már nem módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="38edc-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="38edc-110">Adhatja meg a sourceAnchor értékét egy adott helyszíni AD az objektum, az msDS-ConsistencyGuid attribútumot konfigurálása előtt Azure AD csatlakozás lesz importálva.</span><span class="sxs-lookup"><span data-stu-id="38edc-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="38edc-111">SourceAnchor és ConsistencyGuid további információt talál a következő: [Azure AD csatlakozás: tervezési koncepciók](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="38edc-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

