---
title: A Microsoft Edge speciális hitelesítési koncepciói
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398586"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="1ad90-102">A Microsoft Edge speciális hitelesítési koncepciói</span><span class="sxs-lookup"><span data-stu-id="1ad90-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="1ad90-103">Az alábbiakban a Microsoft Edge-re vonatkozó speciális hitelesítési fogalmakat íme:</span><span class="sxs-lookup"><span data-stu-id="1ad90-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="1ad90-104">**Proaktív hitelesítés**</span><span class="sxs-lookup"><span data-stu-id="1ad90-104">**Proactive Authentication**</span></span>

<span data-ttu-id="1ad90-105">A [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) házirend engedélyezésekor a Microsoft Edge megpróbálja proaktívan hitelesíteni a bejelentkezett felhasználókat a Microsoft-szolgáltatásokon keresztül.</span><span class="sxs-lookup"><span data-stu-id="1ad90-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="1ad90-106">Rendszeres időközönként egy online szolgáltatáson keresztül ellenőrzi a proaktív hitelesítést szabályozó konfigurációt tartalmazó frissített jegyzékfájlt.</span><span class="sxs-lookup"><span data-stu-id="1ad90-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="1ad90-107">Előnyök: A proaktív hitelesítés hitelesítést tesz lehetővé a főbb szolgáltatásoknak, például az Office Új lapnak.</span><span class="sxs-lookup"><span data-stu-id="1ad90-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="1ad90-108">Ha keresőmotorként a Binget használja, a proaktív hitelesítés javítja a címsor teljesítményét, és a vállalat igényeire szabott keresési eredményeket hoz létre.</span><span class="sxs-lookup"><span data-stu-id="1ad90-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="1ad90-109">**Windows Hello CredUI NTLM-hitelesítéshez**</span><span class="sxs-lookup"><span data-stu-id="1ad90-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="1ad90-110">Ha az egyszeri bejelentkezés nem érhető el, amikor egy webhely az NTLM vagy a Egyeztetési mechanizmuson keresztül próbál meg bejelentkezni a felhasználóba, ez a funkció lehetővé teszi, hogy a felhasználó megosztsa az operációs rendszer hitelesítő adatait a webtel, és megfeleljön a hitelesítési kihívásnak a Windows Hello Cred felhasználói felület használatával.</span><span class="sxs-lookup"><span data-stu-id="1ad90-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="1ad90-111">Ez a bejelentkezési folyamat csak a Windows 10-ben fog megjelenni, és csak azok a felhasználók számára, akik nem kapják meg az SSO-t NTLM vagy a negotiate challenge (Kienálás).</span><span class="sxs-lookup"><span data-stu-id="1ad90-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="1ad90-112">**Mentett jelszavak használata az automatikus bejelentkezéshez**</span><span class="sxs-lookup"><span data-stu-id="1ad90-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="1ad90-113">Azok a felhasználók, akik jelszavakat mentnek a Microsoft Edge-ben, engedélyezhetik az automatikus bejelentkezést olyan webhelyekre, amelyekhez hitelesítő adatokat mentettek.</span><span class="sxs-lookup"><span data-stu-id="1ad90-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="1ad90-114">A felhasználók be- vagy kikapcsolhatja ezt a edge://settings/passwords, és a jelszókezelői [házirendek között is konfigurálhatja.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="1ad90-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
