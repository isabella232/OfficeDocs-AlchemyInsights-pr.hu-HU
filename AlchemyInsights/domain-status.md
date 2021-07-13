---
title: Domain Status (Tartomány állapota) – Nincs kijelölt szolgáltatás
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389183"
---
# <a name="domain-status---no-services-selected"></a><span data-ttu-id="56304-102">Domain Status (Tartomány állapota) – Nincs kijelölt szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="56304-102">Domain Status - No services selected</span></span>

<span data-ttu-id="56304-103">**Nincs kijelölt** szolgáltatás, az azt jelenti, hogy nem jelölt ki Microsoft 365-szolgáltatásokat (például Exchange Online, Skype Vállalati verzió vagy Intune, illetve az Microsoft 365 mobileszköz-kezelés az egyéni tartománnyal való használatra).</span><span class="sxs-lookup"><span data-stu-id="56304-103">**No services selected** means you haven’t selected any Microsoft 365 services such as Exchange Online, Skype for Business or Intune, and Mobile Device Management for Microsoft 365 to use with your custom domain.</span></span> <span data-ttu-id="56304-104">Ha hibrid (helyszíni Exchange Exchange Exchange Online) vagy külső levélszemétszűrésben használja az Exchange-et, és más szűrőt Microsoft-szolgáltatások, figyelmen kívül hagyhatja ezt az üzenetet.</span><span class="sxs-lookup"><span data-stu-id="56304-104">If you're using Exchange Hybrid (Exchange on-premises with Exchange Online) or external spam filtering with Exchange and no other Microsoft services, you can ignore this message.</span></span> <span data-ttu-id="56304-105">A tartomány állapota csak a közvetlenül a szolgáltatáshoz csatlakoztatott tartományokhoz érhető el.</span><span class="sxs-lookup"><span data-stu-id="56304-105">Domain health status is available only for domains connected directly to the service.</span></span>

<span data-ttu-id="56304-106">Szolgáltatások kiválasztása a tartományhoz:</span><span class="sxs-lookup"><span data-stu-id="56304-106">To select services for your domain:</span></span>

1. <span data-ttu-id="56304-107">A **Gépház** tartományok csoportban jelölje be a tartomány melletti jelölőnégyzetet a Nincs kijelölt szolgáltatások  >  [](https://admin.microsoft.com/Adminportal/Home) **állapotüzenettel.**</span><span class="sxs-lookup"><span data-stu-id="56304-107">From **Settings** > [**Domains**](https://admin.microsoft.com/Adminportal/Home), check the box next to the domain with the status message **No services selected**.</span></span>
1. <span data-ttu-id="56304-108">A **Dns kezelése lehetőséget** választva indítsa el a Tartománybeállítási varázslót.</span><span class="sxs-lookup"><span data-stu-id="56304-108">Select **Manage DNS** to start the Domain Setup Wizard.</span></span>
    - <span data-ttu-id="56304-109">Ha a **Saját DNS-rekordok hozzáadása lehetőséget választja,** amikor a rendszer kéri, jelöljön ki egy szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="56304-109">If you choose **Add your own DNS records**, be sure to select a service when prompted.</span></span> <span data-ttu-id="56304-110">További szolgáltatások a Speciális beállítások **alatt érhetők el.**</span><span class="sxs-lookup"><span data-stu-id="56304-110">More services could be available under **Advanced Options**.</span></span>
    - <span data-ttu-id="56304-111">Ha A **Microsoft hozzáadhatja** a DNS-rekordjait vagy a További beállítások beállítását választja, a rendszer automatikusan javasolja és kiválasztja az  >  **online** szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="56304-111">If you choose **Let Microsoft add your DNS records** or **More options** > **Setup my online services for me** all available services are suggested and selected automatically.</span></span>
1. <span data-ttu-id="56304-112">Folytassa a varázsló lépéseit a DNS beállításának és a szolgáltatásbeállításoknak a befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="56304-112">Continue through the wizard to complete DNS setup and your service choices.</span></span>
 
<span data-ttu-id="56304-113">A tartomány beállításával kapcsolatos további segítségért lásd: [A tartomány csatlakoztatása DNS-rekordok hozzáadása.](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="56304-113">For additional help setting up your domain, see [Add DNS records to connect your domain](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

