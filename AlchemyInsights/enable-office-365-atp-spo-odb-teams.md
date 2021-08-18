---
title: A Office 365, a SharePoint, a OneDrive és a Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332161"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>A Microsoft Defender engedélyezése Office 365 online SharePoint, OneDrive és Microsoft Teams

1. Jelentkezzen https://protection.office.com be.
2. Válassza **a Veszélyforrások elleni**  >  **Széf**  >  **mellékletek lehetőséget.**
3. Válassza **a Defender bekapcsolás a Office 365, SharePoint, OneDrive és Microsoft Teams** lehetőséget, majd kattintson a Mentés **gombra.**
4. (Ajánlott) Globális rendszergazdaként vagy a SharePoint Online rendszergazdájaként futtassa a [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) parancsmagot úgy, hogy a **DisallowInfectedFileDownload** paraméter értéke *true*.
5. (Ajánlott) [Értesítések beállítása az](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) észlelt fájlokhoz.

**Megjegyzés:** A Microsoft Defender Office 365 nem vizsgálja át az összes fájlt a SharePoint online, OneDrive vagy Microsoft Teams. A fájlokat aszinkron módon, megosztási és vendégtevékenység-eseményeket használó folyamaton keresztül, intelligens heurisztikus és veszélyforrás-észleléssel azonosíthatja a kártékony fájlokat. Lásd: [Microsoft Defender Office 365 a SharePoint, a OneDrive és](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)a Microsoft Teams.
