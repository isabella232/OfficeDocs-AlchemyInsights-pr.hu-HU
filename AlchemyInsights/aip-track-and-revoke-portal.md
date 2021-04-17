---
title: 'AIP: A portál nyomon követése és visszavonása'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002281"
- "5519"
ms.openlocfilehash: b187cd9a0f11168f54deb226c4828c280c0763cd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821593"
---
# <a name="aip-track-and-revoke-portal"></a><span data-ttu-id="391bd-102">AIP: A portál nyomon követése és visszavonása</span><span class="sxs-lookup"><span data-stu-id="391bd-102">AIP: Track and revoke portal</span></span>

<span data-ttu-id="391bd-103">Az Azure Information Protection **használata** esetén az Azure Portalon a dokumentumkövetési webhelyen nyomon követheti és visszavonhatja a dokumentumokat.</span><span class="sxs-lookup"><span data-stu-id="391bd-103">Use the **document tracking site** in the Azure Portal to track and revoke documents when using Azure Information Protection.</span></span> <span data-ttu-id="391bd-104">Az Office-alkalmazások (Word, Excel és PowerPoint) és a Fájlkezelő a dokumentumok nyomon követésére és visszavonására is használhatók.</span><span class="sxs-lookup"><span data-stu-id="391bd-104">The Office applications (Word, Excel and PowerPoint) and File Explorer can also be used to track and revoke documents.</span></span>

1. <span data-ttu-id="391bd-105">A dokumentumkövetési webhelyen kattintson a Hozzáférés **visszavonása elemre.**</span><span class="sxs-lookup"><span data-stu-id="391bd-105">In the document tracking site, click **Revoke access**.</span></span> <span data-ttu-id="391bd-106">Egy dokumentum megfordítása eltávolítja a hozzáférést az engedéllyel rendelkező felhasználóktól; a dokumentum nem törlődik.</span><span class="sxs-lookup"><span data-stu-id="391bd-106">Revoking a document removes access from authorized users; the document is not deleted.</span></span>
2. <span data-ttu-id="391bd-107">Az Office-alkalmazásban:</span><span class="sxs-lookup"><span data-stu-id="391bd-107">In the Office application:</span></span>
    - <span data-ttu-id="391bd-108">Nyissa meg a nyomon követni vagy visszavonni kívánt védett dokumentumot.</span><span class="sxs-lookup"><span data-stu-id="391bd-108">Open the protected document that you want to track or revoke.</span></span>
    - <span data-ttu-id="391bd-109">A Kezdőlap **lap** Védelem csoportjában **kattintson** a Nyomon > **gombra.**</span><span class="sxs-lookup"><span data-stu-id="391bd-109">On the **Home** tab, in the **Protection** group, click **Protect > Track and Revoke**.</span></span>

- <span data-ttu-id="391bd-110">A dokumentumok nyomon követéséről és visszavonásáról további információt a Nyomon [követés és visszavonása oldalon található.](https://docs.microsoft.com/azure/information-protection/rms-client/client-track-revoke)</span><span class="sxs-lookup"><span data-stu-id="391bd-110">For additional information on tracking and revoking a document, see [Track and Revoke](https://docs.microsoft.com/azure/information-protection/rms-client/client-track-revoke).</span></span>

<span data-ttu-id="391bd-111">Ha arra kíváncsi, hogy a PowerShell használatával hogyan kezelheti a dokumentumkövetési webhelyet, milyen naplózási információkra van kíváncsi, tekintse át az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="391bd-111">For information on using PowerShell to manage the document tracking site, logging information, see the following:</span></span>
- [<span data-ttu-id="391bd-112">Felhasználói útmutató: Dokumentumok nyomon követése és visszavonása az Azure Information Protection használata esetén</span><span class="sxs-lookup"><span data-stu-id="391bd-112">User Guide: Track and revoke your documents when you use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-track-revoke)
- [<span data-ttu-id="391bd-113">Rendszergazdai útmutató: Dokumentumkövetés konfigurálása és használata az Azure Information Protection szolgáltatáshoz</span><span class="sxs-lookup"><span data-stu-id="391bd-113">Admin Guide: Configuring and using document tracking for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-document-tracking)
- [<span data-ttu-id="391bd-114">Rights Management -használat licenc</span><span class="sxs-lookup"><span data-stu-id="391bd-114">Rights Management use license</span></span>](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#rights-management-use-license)
- [<span data-ttu-id="391bd-115">Azure Information Protection-előfizetések és -funkciók áttekintése</span><span class="sxs-lookup"><span data-stu-id="391bd-115">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- [<span data-ttu-id="391bd-116">Az Azure Information Protection követelményei</span><span class="sxs-lookup"><span data-stu-id="391bd-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="391bd-117">Rövid útmutató az Azure Information Protectionhez</span><span class="sxs-lookup"><span data-stu-id="391bd-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
