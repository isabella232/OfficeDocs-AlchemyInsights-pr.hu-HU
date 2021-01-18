---
title: Alkalmazásproxy konfigurálása
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885134"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="f5dc0-102">Alkalmazásproxy konfigurálása</span><span class="sxs-lookup"><span data-stu-id="f5dc0-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="f5dc0-103">Az Azure AD-ban az alkalmazásproxy-alkalmazásoknak a helyszíni alkalmazások felhőben való elérhetővé való beállításával kapcsolatban a "How to configure an Application Proxy application" (Alkalmazásproxy-alkalmazás beállítása) és a "How [to configure an Application Proxy application"](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)(Alkalmazásproxy-alkalmazás konfigurálása) között található.</span><span class="sxs-lookup"><span data-stu-id="f5dc0-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="f5dc0-104">Az egyszeri bejelentkezés lehetővé teszi a felhasználóknak, hogy többszöri hitelesítés nélkül is hozzáférjenek egy alkalmazáshoz.</span><span class="sxs-lookup"><span data-stu-id="f5dc0-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="f5dc0-105">Lehetővé teszi az egyetlen hitelesítést a felhőben, az Azure Active Directoryval szemben, és lehetővé teszi, hogy a szolgáltatás vagy összekötő megszemélyesülve a felhasználót az alkalmazás esetleges további hitelesítési kihívásának megoldásában teljesítsen.</span><span class="sxs-lookup"><span data-stu-id="f5dc0-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="f5dc0-106">További információ: Egyszeri bejelentkezés beállítása [alkalmazásproxy-alkalmazáshoz.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)</span><span class="sxs-lookup"><span data-stu-id="f5dc0-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="f5dc0-107">Ebből [a cikkből elháríthatja](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) az új alkalmazásproxy-alkalmazások létrehozásakor gyakran szembesülő problémákat.</span><span class="sxs-lookup"><span data-stu-id="f5dc0-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="f5dc0-108">Ha problémákat okoz a háttér-hitelesítés beállításakor az alkalmazáshoz, előfordulhat, hogy el kell hárítani a [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) kényszeres delegálás konfigurációját az alkalmazásproxyhoz, vagy a probléma megoldásához kövesse az alkalmazás [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) protokollal való konfigurálásához szükséges útmutatást.</span><span class="sxs-lookup"><span data-stu-id="f5dc0-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
