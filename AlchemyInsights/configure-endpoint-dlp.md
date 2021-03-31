---
title: A végpont DLP-beállításainak konfigurálása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402427"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="190da-102">A végpont DLP-beállításainak konfigurálása</span><span class="sxs-lookup"><span data-stu-id="190da-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="190da-103">A Microsoft Endpoint DLP lehetővé teszi a DLP-védelem és -figyelés kibővítését a Windows 10-es eszközökön lévő bizalmas információkra.</span><span class="sxs-lookup"><span data-stu-id="190da-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="190da-104">Az eszközök az eszközkezelésbe való átvezetését követően adatveszteség-megelőzési házirendeket hozhat létre, hogy végrehajtsa a megfelelő műveleteket az elemeken.</span><span class="sxs-lookup"><span data-stu-id="190da-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="190da-105">A Tevékenységkezelővel figyelheti a bizalmas elemek tevékenységét.</span><span class="sxs-lookup"><span data-stu-id="190da-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="190da-106">További információért lásd: [Eszközök bevezetése az eszközkezelésbe](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="190da-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="190da-107">A végponti adatveszteség-megelőzés szolgáltatás első lépései:</span><span class="sxs-lookup"><span data-stu-id="190da-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="190da-108">Ellenőrizze, hogy rendelkezik-e a megfelelő termékváltozatok/előfizetések licencével.</span><span class="sxs-lookup"><span data-stu-id="190da-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="190da-109">További információért lásd: [Termékváltozat/előfizetés licencelés](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="190da-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="190da-110">Ellenőrizze az eszközkezelés engedélyezéséhez, a bevezetési lap eléréséhez, illetve az eszközfigyelés be- és kikapcsolához szükséges engedélyeket.</span><span class="sxs-lookup"><span data-stu-id="190da-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="190da-111">További információért lásd: [Engedélyek](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="190da-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="190da-112">Kövesse az eszközbevezetési folyamatot az eszközök bevezetéséhez az eszközkezelésbe.</span><span class="sxs-lookup"><span data-stu-id="190da-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="190da-113">Ha az Eszközbevezetés (előzetes verzió) lehetőség hiányzik az M365 megfelelőségi **Beállítások** közül, erősítse meg, hogy rendelkezik a fent felsorolt megfelelő licencekkel és engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="190da-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="190da-114">További információért lásd: [Eszközök bevezetése](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="190da-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="190da-115">Adatveszteség-megelőzési házirendek létrehozása a bizalmas elemek védelméhez.</span><span class="sxs-lookup"><span data-stu-id="190da-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="190da-116">További információért lásd: [Végpont DLP-házirend forgatókönyvek](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="190da-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="190da-117">A Microsoft végponti adatveszteség-megelőzés szolgáltatásról további információért lásd: [A Microsoft 365 végponti adatveszteség-megelőzés (előzetes verzió)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="190da-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="190da-118">**Fontos adatgyűjtési lépések, ha támogatás szükséges:**</span><span class="sxs-lookup"><span data-stu-id="190da-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="190da-119">MDATP ügyfél elemző előnézet letöltése innen: [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="190da-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="190da-120">Eszköz futtatása rendszergazdaként a parancsablakból:</span><span class="sxs-lookup"><span data-stu-id="190da-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="190da-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="190da-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="190da-122">Amikor az "Adja meg a nyomkövetési percek számát:" kérés jelenik meg, adja meg, hogy hány perc szükséges az eset futtatásához.</span><span class="sxs-lookup"><span data-stu-id="190da-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="190da-123">Eset futtatása</span><span class="sxs-lookup"><span data-stu-id="190da-123">Run the scenario</span></span>

<span data-ttu-id="190da-124">Gyűjtse össze a támogatási szakembernek adandó zip fájl kimenetét.</span><span class="sxs-lookup"><span data-stu-id="190da-124">Collect the Zip file output to be given to the Support agent.</span></span>
