---
title: A Microsoft Edge-re vonatkozó speciális hitelesítési fogalmak
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573521"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="fa5f1-102">A Microsoft Edge-re vonatkozó speciális hitelesítési fogalmak</span><span class="sxs-lookup"><span data-stu-id="fa5f1-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="fa5f1-103">A Microsoft Edge-re vonatkozó speciális hitelesítési fogalmak a következők:</span><span class="sxs-lookup"><span data-stu-id="fa5f1-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="fa5f1-104">**Proaktív hitelesítés**</span><span class="sxs-lookup"><span data-stu-id="fa5f1-104">**Proactive Authentication**</span></span>

<span data-ttu-id="fa5f1-105">Ha engedélyezi a [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -házirendet, a Microsoft Edge megpróbálja proaktívan hitelesíteni a bejelentkezett felhasználókat a Microsoft Services szolgáltatáson keresztül.</span><span class="sxs-lookup"><span data-stu-id="fa5f1-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="fa5f1-106">Rendszeres időközönként egy online szolgáltatással ellenőrizheti, hogy egy olyan frissített jegyzékfájlt szeretne-e használni, amely a proaktív hitelesítésre vonatkozó konfigurációt tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="fa5f1-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="fa5f1-107">Előnyök: a proaktív hitelesítés a legfontosabb szolgáltatásokhoz (például az Office új lap lapjához) való hitelesítést engedélyezi.</span><span class="sxs-lookup"><span data-stu-id="fa5f1-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="fa5f1-108">Ha a Bing a keresőmotorként van használatban, a proaktív hitelesítés javítja a címsor működését, és segít a keresés eredményének a vállalati igényekhez való személyre szabásában.</span><span class="sxs-lookup"><span data-stu-id="fa5f1-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="fa5f1-109">**Windows Hello CredUI NTLM-hitelesítéshez**</span><span class="sxs-lookup"><span data-stu-id="fa5f1-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="fa5f1-110">Ha az egyszeri bejelentkezés (SSO) nem érhető el, ha egy webhely az NTLM vagy az egyeztetési mechanizmuson keresztül próbál meg bekapcsolódni a felhasználóhoz, ez a funkció lehetővé teszi, hogy a felhasználó megossza az operációs rendszer hitelesítő adatait a webhellyel, és a Windows Hello cred felhasználói felülete segítségével kielégítse a hitelesítési kihívást.</span><span class="sxs-lookup"><span data-stu-id="fa5f1-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="fa5f1-111">Ez a bejelentkezési folyamat csak a Windows 10 rendszerben jelenik meg, és csak azoknál a felhasználóknál, akik NTLM-vagy értekezlet-összehívási probléma esetén nem kapnak SSO-t.</span><span class="sxs-lookup"><span data-stu-id="fa5f1-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="fa5f1-112">**A mentett jelszavak használata automatikusan történő bejelentkezéshez**</span><span class="sxs-lookup"><span data-stu-id="fa5f1-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="fa5f1-113">Azok a felhasználók, akik a Microsoft Edge-ben mentették a jelszavakat, engedélyezhetik az automatikus bejelentkezést olyan webhelyekre, ahol a hitelesítő adatok találhatók.</span><span class="sxs-lookup"><span data-stu-id="fa5f1-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="fa5f1-114">A felhasználók a edge://settings/passwords-ban be-vagy kikapcsolhatja ezt a funkcióját, és a [jelszó-kezelő](https://go.microsoft.com/fwlink/?linkid=2134622) házirendben is konfigurálhatók.</span><span class="sxs-lookup"><span data-stu-id="fa5f1-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
