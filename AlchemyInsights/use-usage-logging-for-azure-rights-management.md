---
title: Használati naplózás használata az Azure Rights Management hez
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555545"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="5c41b-102">Használati naplózás használata az Azure Rights Management hez</span><span class="sxs-lookup"><span data-stu-id="5c41b-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="5c41b-103">Alapértelmezés szerint a védelmi használat naplózása minden ügyfél számára engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="5c41b-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="5c41b-104">A naplók blobok sorozataként vannak megírva az Azure storage-ban a bérlő számára.</span><span class="sxs-lookup"><span data-stu-id="5c41b-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="5c41b-105">Egy védelmi művelet után akár 15 percet is igénybe vehet, amíg a legtöbb napló megjelenik.</span><span class="sxs-lookup"><span data-stu-id="5c41b-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="5c41b-106">A védelmi használati naplók segítségével:</span><span class="sxs-lookup"><span data-stu-id="5c41b-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="5c41b-107">Üzleti elemzések elemzése</span><span class="sxs-lookup"><span data-stu-id="5c41b-107">Analyze business insights</span></span>

- <span data-ttu-id="5c41b-108">A visszaélések figyelése</span><span class="sxs-lookup"><span data-stu-id="5c41b-108">Monitor for abuse</span></span>

- <span data-ttu-id="5c41b-109">Kriminalisztikai elemzés elvégzése</span><span class="sxs-lookup"><span data-stu-id="5c41b-109">Perform forensic analysis</span></span>

<span data-ttu-id="5c41b-110">További információ: [Naplózás és az Azure Information Protection védelmi használatának elemzése.](https://docs.microsoft.com/azure/information-protection/log-analyze-usage)</span><span class="sxs-lookup"><span data-stu-id="5c41b-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="5c41b-111">Az ügyfélhasználat naplózásáról további információt a [Felügyeleti útmutató: Azure Information Protection ügyfélfájlok és ügyfélhasználat-naplózás című témakörben talál.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging)</span><span class="sxs-lookup"><span data-stu-id="5c41b-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="5c41b-112">További információ:</span><span class="sxs-lookup"><span data-stu-id="5c41b-112">For additional information, see:</span></span>

- <span data-ttu-id="5c41b-113">[Az Azure Information Protection követelményei](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="5c41b-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="5c41b-114">[Oktatóanyag: Konfigurálja az Azure Information Protection házirend-beállításait, és hozzon létre egy új címkét.](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)</span><span class="sxs-lookup"><span data-stu-id="5c41b-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>