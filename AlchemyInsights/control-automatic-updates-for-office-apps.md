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
# <a name="control-automatic-updates-for-office-apps"></a>Az Office Apps automatikus frissítéseinek szabályozása

Alapértelmezés szerint az Office-alkalmazások frissítései automatikusan letöltődnek, és a háttérben, felhasználói beavatkozás nélkül kerülnek alkalmazásra. A rendszergazdák azonban az Office Update beállításaival szabályozhatják a frissítések alkalmazásának módját. A frissítési beállítások lehetővé teszik a rendszergazdák számára az automatikus frissítések engedélyezését vagy letiltását, a **Frissítés gomb** megjelenítését vagy elrejtését az Office-ban, a frissítési határidők beállítását stb. Részletes információkért lásd:

- [Az Office frissítési beállításainak konfigurálása](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Az Office automatikus frissítése nincs engedélyezve](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Az Office frissítésének meghatározása a telepítés után](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Az ügyfélgépre alkalmazott meglévő frissítési beállítások áttekintéséhez hajtsa végre az alábbi lépéseket:

1. Nyissa meg a Rendszerleíróadatbázis-szerkesztőt a Start Run regedit **(Futtatás indítás)**  >  **Run**  >  **beállítási programban.**
2. Váltson a következő helyre, és tekintse át az Office Update beállításait:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Megjegyzés:**  Ha az OfficeMgmtCOM kulcs be van állítva, az **Office**  >  **Fiók**  >  **Office-frissítések**című témakörben a "A rendszergazdák által kezelt frissítések" üzenet jelenhet meg. További információt a [Microsoft 365-alkalmazások frissítéseinek kezelése a Microsoft Endpoint Configuration Manager alkalmazással (Microsoft Endpoint Configuration Manager) témakörben talál.](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)  