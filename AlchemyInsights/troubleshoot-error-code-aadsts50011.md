---
title: Az AADSTS50011 hibakód hibaelhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036667"
---
# <a name="troubleshoot-error-code-aadsts50011"></a><span data-ttu-id="c7fd3-102">Az AADSTS50011 hibakód hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="c7fd3-102">Troubleshoot error code AADSTS50011</span></span>

<span data-ttu-id="c7fd3-103">Az AADSTS50011-es hiba elhárításához végezze el az alábbi ajánlott lépést.</span><span class="sxs-lookup"><span data-stu-id="c7fd3-103">To resolve AADSTS50011 error, perform the recommended step described below.</span></span>

<span data-ttu-id="c7fd3-104">**AADSTS50011:** InvalidReplyTo – A válaszcím hiányzik, helytelenül van beállítva, vagy nem egyezik az apphoz konfigurált válaszcímekkel.</span><span class="sxs-lookup"><span data-stu-id="c7fd3-104">**AADSTS50011**: InvalidReplyTo - The reply address is missing, misconfigured, or does not match reply addresses configured for the app.</span></span>

<span data-ttu-id="c7fd3-105">A probléma megoldásaként vegye fel ezt a hiányzó válaszcímet az Azure Active Directory (AD) appba, vagy vegyen fel valakit, aki rendelkezik az alkalmazás AD-ban való kezeléséhez szükséges engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="c7fd3-105">As a resolution ensure to add this missing reply address to the Azure Active Directory (AD) app or have someone with the permissions to manage your application in AD do this for you.</span></span> <span data-ttu-id="c7fd3-106">További információt az [AADSTS50011-es](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch)hibaelhárító cikkben talál.</span><span class="sxs-lookup"><span data-stu-id="c7fd3-106">For more information, see the troubleshooting article for error [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span></span>