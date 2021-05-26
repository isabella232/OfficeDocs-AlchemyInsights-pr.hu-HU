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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657931"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="6db19-102">A végpont DLP-beállításainak konfigurálása</span><span class="sxs-lookup"><span data-stu-id="6db19-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="6db19-103">A Microsoft Endpoint DLP lehetővé teszi a DLP-védelem és -figyelés kibővítését a Windows 10-es eszközökön lévő bizalmas információkra.</span><span class="sxs-lookup"><span data-stu-id="6db19-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="6db19-104">Az eszközök az eszközkezelésbe való átvezetését követően adatveszteség-megelőzési házirendeket hozhat létre, hogy végrehajtsa a megfelelő műveleteket az elemeken.</span><span class="sxs-lookup"><span data-stu-id="6db19-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="6db19-105">A Tevékenységkezelővel figyelheti a bizalmas elemek tevékenységét.</span><span class="sxs-lookup"><span data-stu-id="6db19-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="6db19-106">További információért lásd: [Eszközök bevezetése az eszközkezelésbe](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="6db19-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="6db19-107">A végponti adatveszteség-megelőzés szolgáltatás első lépései:</span><span class="sxs-lookup"><span data-stu-id="6db19-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="6db19-108">Ellenőrizze, hogy rendelkezik-e a megfelelő termékváltozatok/előfizetések licencével.</span><span class="sxs-lookup"><span data-stu-id="6db19-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="6db19-109">További információért lásd: [Termékváltozat/előfizetés licencelés](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="6db19-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="6db19-110">Ellenőrizze az eszközkezelés engedélyezéséhez, a bevezetési lap eléréséhez, illetve az eszközfigyelés be- és kikapcsolához szükséges engedélyeket.</span><span class="sxs-lookup"><span data-stu-id="6db19-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="6db19-111">További információért lásd: [Engedélyek](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="6db19-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="6db19-112">Kövesse az eszközbevezetési folyamatot az eszközök bevezetéséhez az eszközkezelésbe.</span><span class="sxs-lookup"><span data-stu-id="6db19-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="6db19-113">További információért lásd: [Eszközök bevezetése](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="6db19-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="6db19-114">Adatveszteség-megelőzési házirendek létrehozása a bizalmas elemek védelméhez.</span><span class="sxs-lookup"><span data-stu-id="6db19-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="6db19-115">További információért lásd: [Végpont DLP-házirend forgatókönyvek](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="6db19-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="6db19-116">A Microsoft végponti adatveszteség-megelőzés szolgáltatásról további információért lásd: [A Microsoft 365 végponti adatveszteség-megelőzés (előzetes verzió)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="6db19-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="6db19-117">**Fontos adatgyűjtési lépések, ha támogatás szükséges:**</span><span class="sxs-lookup"><span data-stu-id="6db19-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="6db19-118">Töltse [MDATP Client Analyzer Preview (Ügyfélanalizáló előzetes verzió) gombra.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="6db19-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="6db19-119">Eszköz futtatása rendszergazdaként a parancsablakból:</span><span class="sxs-lookup"><span data-stu-id="6db19-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="6db19-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="6db19-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="6db19-121">Amikor a rendszer **kéri, adja** meg a nyomkövetések gyűjtéséhez szükséges percek számát: , adja meg az eset futtatásához szükséges percek számát.</span><span class="sxs-lookup"><span data-stu-id="6db19-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="6db19-122">Futtassa az esetet.</span><span class="sxs-lookup"><span data-stu-id="6db19-122">Run the scenario.</span></span>

<span data-ttu-id="6db19-123">Gyűjtse össze a Zip-fájl kimenetét, és adja át a támogatási ügynöknek.</span><span class="sxs-lookup"><span data-stu-id="6db19-123">Collect the Zip file output to give to the Support agent.</span></span>
