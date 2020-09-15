---
title: Az Office 365 ATP engedélyezése a SharePointhoz, a OneDrive és a Microsoft Teams alkalmazáshoz
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709909"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Az Office 365 Advanced Threat Protection engedélyezése a SharePoint Online, a OneDrive és a Microsoft Teams esetében

1. Ugrás https://protection.office.com és bejelentkezés.
2. Válassza a **veszélyforrások kezelése**a  >  **Policy**  >  **biztonságos mellékleteket**.
3. Jelölje be **az ATP bekapcsolása a sharepointhoz, a OneDrive és a Microsoft Teams**jelölőnégyzetet, és kattintson a **Mentés**gombra.
4. Ajánlott Globális rendszergazdaként vagy SharePoint Online-rendszergazdaként futtassa a [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) parancsmagot a **DisallowInfectedFileDownload** paraméter *true*értékre állításával.
5. Ajánlott Az észlelt fájlokra vonatkozó [értesítések beállítása](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) .

> [!NOTE]
> Az ATP a SharePoint Online, a OneDrive vagy a Microsoft Teams minden egyes fájljának beolvasását fogja tartalmazni. A fájlok egy-egy megosztási és vendég-tevékenységi eseményeket használó folyamaton keresztül, valamint intelligens heurisztikus és veszélyforrás jelzésekkel beolvassák a kártékony fájlokat. Lásd: [ATP for SharePoint, OneDrive és Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).