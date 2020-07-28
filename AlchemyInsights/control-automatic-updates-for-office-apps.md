---
title: Az Office Apps automatikus frissítéseinek szabályozása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439333"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="5e50c-102">Az Office Apps automatikus frissítéseinek szabályozása</span><span class="sxs-lookup"><span data-stu-id="5e50c-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="5e50c-103">Alapértelmezés szerint az Office-alkalmazások frissítései automatikusan letöltődnek, és a háttérben, felhasználói beavatkozás nélkül kerülnek alkalmazásra.</span><span class="sxs-lookup"><span data-stu-id="5e50c-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="5e50c-104">A rendszergazdák azonban az Office Update beállításaival szabályozhatják a frissítések alkalmazásának módját.</span><span class="sxs-lookup"><span data-stu-id="5e50c-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="5e50c-105">A frissítési beállítások lehetővé teszik a rendszergazdák számára az automatikus frissítések engedélyezését vagy letiltását, a **Frissítés gomb** megjelenítését vagy elrejtését az Office-ban, a frissítési határidők beállítását stb.</span><span class="sxs-lookup"><span data-stu-id="5e50c-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="5e50c-106">Részletes információkért lásd:</span><span class="sxs-lookup"><span data-stu-id="5e50c-106">For detailed information, see:</span></span>

- [<span data-ttu-id="5e50c-107">Az Office frissítési beállításainak konfigurálása</span><span class="sxs-lookup"><span data-stu-id="5e50c-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="5e50c-108">Az Office automatikus frissítése nincs engedélyezve</span><span class="sxs-lookup"><span data-stu-id="5e50c-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="5e50c-109">Az Office frissítésének meghatározása a telepítés után</span><span class="sxs-lookup"><span data-stu-id="5e50c-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="5e50c-110">Az ügyfélgépre alkalmazott meglévő frissítési beállítások áttekintéséhez hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="5e50c-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="5e50c-111">Nyissa meg a Rendszerleíróadatbázis-szerkesztőt a Start Run regedit **(Futtatás indítás)**  >  **Run**  >  **beállítási programban.**</span><span class="sxs-lookup"><span data-stu-id="5e50c-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="5e50c-112">Váltson a következő helyre, és tekintse át az Office Update beállításait:</span><span class="sxs-lookup"><span data-stu-id="5e50c-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="5e50c-113">a.</span><span class="sxs-lookup"><span data-stu-id="5e50c-113">a.</span></span> <span data-ttu-id="5e50c-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="5e50c-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="5e50c-115">b.</span><span class="sxs-lookup"><span data-stu-id="5e50c-115">b.</span></span> <span data-ttu-id="5e50c-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="5e50c-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="5e50c-117">**Megjegyzés:**  Ha az OfficeMgmtCOM kulcs be van állítva, az **Office**  >  **Fiók**  >  **Office-frissítések**című témakörben a "A rendszergazdák által kezelt frissítések" üzenet jelenhet meg.</span><span class="sxs-lookup"><span data-stu-id="5e50c-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="5e50c-118">További információt a [Microsoft 365-alkalmazások frissítéseinek kezelése a Microsoft Endpoint Configuration Manager alkalmazással (Microsoft Endpoint Configuration Manager) témakörben talál.](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)</span><span class="sxs-lookup"><span data-stu-id="5e50c-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  