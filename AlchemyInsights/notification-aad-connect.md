---
title: Értesítés az AAD Connectről
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036110"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="6a0ef-102">Értesítés az AAD Connectről</span><span class="sxs-lookup"><span data-stu-id="6a0ef-102">Notification AAD Connect</span></span>

- <span data-ttu-id="6a0ef-103">Győződjön meg arról, hogy jogosult a művelet elvégzésére.</span><span class="sxs-lookup"><span data-stu-id="6a0ef-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="6a0ef-104">A globális rendszergazdáknak alapértelmezés szerint van hozzáférésük.</span><span class="sxs-lookup"><span data-stu-id="6a0ef-104">Global Admins have access by default.</span></span> <span data-ttu-id="6a0ef-105">A szerepköralapú hozzáférés-vezérlési szolgáltatásokkal ezenkívül delegálhatja a regisztrálási engedélyeket a közreműködőnek. [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="6a0ef-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="6a0ef-106">Győződjön meg arról, hogy a szükséges végpontok engedélyezve vannak, és nem blokkolva vannak a tűzfal miatt.</span><span class="sxs-lookup"><span data-stu-id="6a0ef-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="6a0ef-107">Részletes információkért lásd: [követelmények.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="6a0ef-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="6a0ef-108">A regisztráció meghiúsulhat, mert a kimenő kommunikációt a hálózati réteg SSL-vizsgálatnak kell átesni.</span><span class="sxs-lookup"><span data-stu-id="6a0ef-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="6a0ef-109">Ellenőrizze, hogy ellenőrizte-e az Azure AD Connect Health értesítési beállításait, és ellenőrizze a beállítást.</span><span class="sxs-lookup"><span data-stu-id="6a0ef-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="6a0ef-110">Az Azure AD Connect Health értesítési beállításainak konfigurálásról ebben az útmutatóban [kaphat útmutatást.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="6a0ef-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="6a0ef-111">Ha többet szeretne tudni az AAD Connect Health szinkronizálási jelentésről és letöltésről, olvassa el az [Objektumszintű szinkronizálási jelentés .](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="6a0ef-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="6a0ef-112">Az AAD Connect Health Alerts hibaelhárítási útmutatóját kövesse az [AAD Connect health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) (Állapot-állapot) állapotjelzésekkel kapcsolatos hibaelhárítási útmutatóban, valamint a gyakori kérdésekre az [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)telepítésével kapcsolatos gyakori kérdések között.</span><span class="sxs-lookup"><span data-stu-id="6a0ef-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
