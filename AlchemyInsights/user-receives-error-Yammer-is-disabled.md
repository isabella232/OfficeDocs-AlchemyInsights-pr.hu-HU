---
title: 'A felhasználó hibaüzenetet kap: AADSTS7000112 Yammer le van tiltva'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198057"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="9e1fe-102">A felhasználó hibaüzenetet kap: AADSTS7000112 Yammer le van tiltva</span><span class="sxs-lookup"><span data-stu-id="9e1fe-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="9e1fe-103">Ha az "AADSTS7000112: Application '000000005-0000-0ff1-000000000000000"(Yammer) le van tiltva" hibaüzenet jelenik meg, probléma van az Azure AD szolgáltatásfőelemével.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="9e1fe-104">Előfordulhat, hogy egy rendszergazda letiltotta az egyszerű szolgáltatást a Yammerhez való hozzáférés letiltásához.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="9e1fe-105">A szolgáltatásnév letiltása nem ajánlott, és további problémákat okozhat.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="9e1fe-106">A Yammer felhasználói hozzáférésének letiltására vonatkozó támogatott módszerről a [Yammer-hozzáférés kikapcsolása a Microsoft 365-felhasználók számára](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)című témakörben talál további információt.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="9e1fe-107">A probléma kijavítása az Azure Portalon, és a Yammer felhasználói hozzáférésének visszaállítása:</span><span class="sxs-lookup"><span data-stu-id="9e1fe-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="9e1fe-108">Nyissa meg az Azure Active Directory lapot, és válassza **a Vállalati alkalmazások** **csoportban a bal** oldali navigációs ablakban.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="9e1fe-109">Írja be az **Office 365 Yammer kifejezést** a keresőmezőbe, és válassza ki az alkalmazás nevét a beállítások megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="9e1fe-110">A bal oldali navigációs ablakban válassza a **Tulajdonságok** lehetőséget a **Kezelés** csoportban.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="9e1fe-111">Állítsa be a felhasználók számára engedélyezve a **bejelentkezéshez jelölőnégyzetet,** majd válassza **a** **Mentés**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="9e1fe-112">Jelentkezzen be ismét a Yammerbe.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-112">Sign in to Yammer again.</span></span> <span data-ttu-id="9e1fe-113">Előfordulhat, hogy törölnie kell a cookie-kat.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-113">You might need to clear cookies.</span></span>

<span data-ttu-id="9e1fe-114">Másik lehetőségként futtassa a PowerShell-parancsokat az érték beállításához.</span><span class="sxs-lookup"><span data-stu-id="9e1fe-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="9e1fe-115">További információt a ["Sajnáljuk, de nem sikerül bejelentkeznünk" hibaüzenet jelenik meg, amikor az Office 365 Yammer csempéjére kattint.](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="9e1fe-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 