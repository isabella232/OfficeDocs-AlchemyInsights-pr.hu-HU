---
title: Nem lehet bejelentkezni a Teamsbe az autologon.microsoftazuread-sso.com:443 hiba miatt
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932043"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="fa119-102">Nem lehet bejelentkezni a Teamsbe az autologon.microsoftazuread-sso dot com:443 hiba miatt</span><span class="sxs-lookup"><span data-stu-id="fa119-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="fa119-103">Ha közvetlen egyszeri bejelentkezés engedélyezett az Office 365-ös hitelesítésként, előfordulhat, hogy az „autologon.microsoftazuread-sso.com” URL-címet hozzá kell adni az intranetes helyekhez.</span><span class="sxs-lookup"><span data-stu-id="fa119-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="fa119-104">Ha már korábban hozzáadta a megbízható helyekhez, és közvetlen egyszeri bejelentkezést használ, el kell távolítania a megbízható helyek közül.</span><span class="sxs-lookup"><span data-stu-id="fa119-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="fa119-105">Tanulmányozza a [közvetlen egyszeri bejelentkezés hibaelhárítási ellenőrzőlistáját](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="fa119-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="fa119-106">Ezeket a lépéseket követve vegyen fel URL-címeket az intranetes helyek listájára:</span><span class="sxs-lookup"><span data-stu-id="fa119-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="fa119-107">A **Start** gombra kattintva nyissa meg az Internet Explorert.</span><span class="sxs-lookup"><span data-stu-id="fa119-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="fa119-108">A keresőmezőbe írja be az Internet Explorer nevet, majd a találatok listájában kattintson az **Internet Explorer** elemre.</span><span class="sxs-lookup"><span data-stu-id="fa119-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="fa119-109">Válassza az **Eszközök** menü **Internetbeállítások** parancsát.</span><span class="sxs-lookup"><span data-stu-id="fa119-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="fa119-110">Kattintson a **Biztonság** fülre.</span><span class="sxs-lookup"><span data-stu-id="fa119-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="fa119-111">Ezután kattintson a **Helyi intranet** ikonra, majd a **Helyek** gombra, végül a **Speciális** gombra.</span><span class="sxs-lookup"><span data-stu-id="fa119-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="fa119-112">Adja meg a webhely URL-címét, és kattintson a **Hozzáadás** gombra.</span><span class="sxs-lookup"><span data-stu-id="fa119-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="fa119-113">Amikor elkészült, kattintson a **Bezárás** gombra.</span><span class="sxs-lookup"><span data-stu-id="fa119-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="fa119-114">További információt a [közvetlen egyszeri bejelentkezés Office 365-höz való telepítésének dokumentációjában](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) talál (a 3. lépés az URL-cím intranetes helyekhez való hozzáadásának házirendalapú eljárását tartalmazza).</span><span class="sxs-lookup"><span data-stu-id="fa119-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
