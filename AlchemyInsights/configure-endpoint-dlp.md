---
title: Végpont DLP konfigurálása
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
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555558"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="cd2b8-102">Végpont DLP konfigurálása</span><span class="sxs-lookup"><span data-stu-id="cd2b8-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="cd2b8-103">A Microsoft Endpoint DLP lehetővé teszi a DLP-védelem és figyelés imázsának kiterjesztését a Windows 10-es eszközök bizalmas adataira.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="cd2b8-104">Miután az eszközök be vannak építve az eszközkezelésbe, DLP-házirendeket hozhat létre az elemek védelmi műveletek kényszerítéséhez.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="cd2b8-105">A Tevékenységkezelő segítségével figyelheti a bizalmas elemek tevékenységét.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="cd2b8-106">További információ: [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="cd2b8-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="cd2b8-107">Az Endpoint DLP első lépései:</span><span class="sxs-lookup"><span data-stu-id="cd2b8-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="cd2b8-108">Győződjön meg arról, hogy rendelkezik a megfelelő Termékváltozat/előfizetések licencelésével.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="cd2b8-109">További információ: [Termékváltozat/előfizetések licencelése.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)</span><span class="sxs-lookup"><span data-stu-id="cd2b8-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="cd2b8-110">Ellenőrizze az eszközkezelés engedélyezéséhez, a bevezetési lap eléréséhez vagy az eszközfigyelés be- és kikapcsolásához szükséges engedélyeket.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="cd2b8-111">További információt az Engedélyek című [témakörben talál.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)</span><span class="sxs-lookup"><span data-stu-id="cd2b8-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="cd2b8-112">Az eszközök beépítése az Eszközkezelésbe a bevezetési eszközök eljárásának követésével.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="cd2b8-113">Ha hiányzik az Eszköz bevezetés (előzetes verzió) opció az M365 megfelelőségi **beállítások**területen, ellenőrizze, hogy rendelkezik-e a fent hivatkozott megfelelő licenccel és engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="cd2b8-114">További [információ: Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="cd2b8-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="cd2b8-115">Hozzon létre DLP-házirendeket a bizalmas elemek védelmére.</span><span class="sxs-lookup"><span data-stu-id="cd2b8-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="cd2b8-116">További információt az [Endpoint DLP-házirend-forgatókönyvek című témakörben talál.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)</span><span class="sxs-lookup"><span data-stu-id="cd2b8-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="cd2b8-117">A Microsoft Endpoint DLP szolgáltatásról további információt a [Microsoft 365 Végpontok adatvesztésének megelőzéséről (előzetes verzió) című témakörben talál.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)</span><span class="sxs-lookup"><span data-stu-id="cd2b8-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>