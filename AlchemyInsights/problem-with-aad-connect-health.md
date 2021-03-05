---
title: Probléma az AAD Connect Health alkalmazással
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482068"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="55774-102">Probléma az AAD Connect Health alkalmazással</span><span class="sxs-lookup"><span data-stu-id="55774-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="55774-103">Győződjön meg arról, hogy jogosult a művelet elvégzésére.</span><span class="sxs-lookup"><span data-stu-id="55774-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="55774-104">A globális rendszergazdáknak alapértelmezés szerint van hozzáférésük.</span><span class="sxs-lookup"><span data-stu-id="55774-104">Global Admins have access by default.</span></span> <span data-ttu-id="55774-105">A szerepköralapú hozzáférés-vezérléssel ezenkívül a közreműködői jogosultságot is delegálhatja. [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="55774-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="55774-106">Győződjön meg arról, hogy a szükséges végpontok engedélyezve vannak, és nem blokkolva vannak a tűzfal miatt.</span><span class="sxs-lookup"><span data-stu-id="55774-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="55774-107">Részletes információkért lásd a [követelményeket.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="55774-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="55774-108">A regisztráció meghiúsulhat, mert a kimenő kommunikációt a hálózati réteg SSL-vizsgálatnak kell átesni.</span><span class="sxs-lookup"><span data-stu-id="55774-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="55774-109">Győződjön meg arról, hogy ellenőrizte az Azure AD Connect Health értesítési beállításait.</span><span class="sxs-lookup"><span data-stu-id="55774-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="55774-110">Kérjük, tekintse át a beállítást.</span><span class="sxs-lookup"><span data-stu-id="55774-110">Please review your setting.</span></span> <span data-ttu-id="55774-111">Ez [az](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) útmutató segítséget ad az Azure AD Connect állapotértesítések értesítési beállításainak konfigurálásában.</span><span class="sxs-lookup"><span data-stu-id="55774-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="55774-112">Az AAD Connect Health szinkronizálási jelentésről és a letöltésről további információt az Objektumszintű szinkronizálási [jelentésben olvashat.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="55774-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="55774-113">Az AAD Connect Health riasztásokkal kapcsolatos hibák elhárításához kövesse az [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) frissességi riasztásokkal kapcsolatos hibaelhárítási útmutatóját, valamint a gyakori kérdéseket az [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)telepítésével kapcsolatos gyakori kérdések között.</span><span class="sxs-lookup"><span data-stu-id="55774-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
