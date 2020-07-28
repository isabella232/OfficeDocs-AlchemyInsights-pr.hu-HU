---
title: Az Office-alkalmazások frissítési csatornáinak módosítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439389"
---
# <a name="change-update-channels-for-office-apps"></a>Az Office-alkalmazások frissítési csatornáinak módosítása

Új Office-telepítések esetén az Office szoftverletöltési beállításai val jelölheti ki a kívánt frissítési csatornát, majd telepítse (vagy telepítse újra) az Office-alkalmazásokat. További információt a [Szoftverletöltési beállítások kezelése az Office 365-ben ( Szoftverletöltési beállítások kezelése ) témakörben talál.](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365) 

**Megjegyzés:** Az Office szoftverletöltési beállításai val kiválasztott frissítési csatorna minden olyan felhasználóra vonatkozik, aki új telepítést hajt végre az O365 portálon. További információt a [Microsoft 365 vagy az Office 2019 letöltése vagy újratelepítése PC-re vagy Mac gépre című témakörben talál.](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)   

Meglévő Office-telepítések esetén az Office-telepítő eszközzel (ODT) másik frissítési csatornára válthat:  

1. Töltse le az Office telepítőeszköz (setup.exe) legújabb verzióját a [Microsoft letöltőközpontjából.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
2. Azonosítsa annak a csatornának a nevét, amelyre váltani szeretne. További információt [az Office-telepítőeszköz konfigurációs beállításai című témakörben talál.](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)
3. Hozzon létre egy konfigurációs XML-fájlt, amely megadja a megfelelő csatornanevet, például update.xml.  
    a. <Configuration>  
    b. <Frissítések **Channel ="Havi"** />  
    c. </Configuration>
4. Rendszergazda jogú parancssorból váltson arra a mappára, ahol setup.exe található, és futtassa a következő parancsot:  
    a. setup.exe /configure update.xml
5. Indítson el egy Office-alkalmazást (például az Excelt), majd válassza a **File**  >  **Fájlfiók**lehetőséget. A Termékinformáció csoportban válassza a **Frissítési beállítások**  >  **frissítése most**lehetőséget.

További információt a [Meglévő Office-alkalmazások frissítési csatornáinak váltása című témakörben talál.](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel) 

A felhasználók egy kiválasztott csoportjának frissítési csatornáinak váltásához vagy a Configuration Manager (SCCM) használatával konfigurálja a Csatorna frissítése beállítást a csoportházirend-azonosító használatával. További információt a [Microsoft 365-alkalmazások frissítési csatornáinak áttekintése című témakörben talál.](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy) További információt Az [Office 365 ProPlus-csatornák informatikai szakembereknek való kezelése](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) és a Microsoft [365-alkalmazások frissítéseinek kezelése a Microsoft Endpoint Configuration Manager rel.](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)