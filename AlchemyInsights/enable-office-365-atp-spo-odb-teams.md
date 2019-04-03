---
title: A SharePoint, a OneDrive és a csapatok a Microsoft Office 365 ATP engedélyezése
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030990"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, a OneDrive és a csapatok a Microsoft Office 365 speciális fenyegetés védelem engedélyezése

1. Ugrás a https://protection.office.com és jelentkezzen be.
2. Válassza ki a **fenyegetés kezelése** > **politika** > **Biztonságos mellékletek**.
3. Válassza az **Ígérethez rendelkezésre álló mennyiség, a SharePoint, a OneDrive, és a Microsoft csapatok**, és kattintson a **Mentés**gombra.
4. (Ajánlott) A globális rendszergazda vagy a SharePoint Online rendszergazdaként futtassa a [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) parancsmaggal a **DisallowInfectedFileDownload** paraméter értéke *true*.
5. (Ajánlott) [Értesítések beállítása](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) a talált fájlokat.

> [!NOTE]
> ATP lesz nto vizsgálat minden SharePoint Online, a OneDrive vagy a Microsoft Teams egyetlen fájlban. Fájlok megosztása és a Vendég tevékenység események, intelligens heurisztikus és rosszindulatú fájlok azonosítása veszély jelek használó folyamat aszinkron módon ellenőrzi. Lásd: [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).