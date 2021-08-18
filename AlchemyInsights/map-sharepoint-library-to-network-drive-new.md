---
title: Tár SharePoint hálózati meghajtóhoz
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: cd3d7d272552d5cd3f21f41160522001d79339d84a6d2259e1b1868deee66ef0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54087246"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>Tár SharePoint hálózati meghajtóhoz

Hálózati meghajtó hozzárendelése helyett szinkronizálja a SharePoint az új ügyfélalkalmazással OneDrive szinkronizálási app igény szerinti fájlokat biztosít. A OneDrive-ban lévő összes fájl elérése helyi tárterület használata nélkül. További információért lásd: [SharePoint-](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) és Teams-fájlok szinkronizálása a számítógépen és Lemezterület megtakarítása az [OneDrive](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)Igény szerinti fájlok igény szerinti Windows 10.

Ha úgy dönt, hogy az új ügyfélprogram helyett egy meghajtót [OneDrive szinkronizálási app](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)meg, kövesse az alábbi lépéseket:

- [A SharePoint Online-hoz csatlakoztatott leképezett hálózati meghajtók hibáinak elhárítása](/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [Hitelesítési hibák akkor fordulnak elő, ha az ügyfél nem támogatja a TLS 1.2-es használatát](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**MEGJEGYZÉS:** Ha a Internet Explorer 10-ot az Windows 8-es vagy a Windows 7-es,  és a hozzáférés megtagadva vagy az Elérési út nem érhető el egy meghajtó megfeleltetésekor, a gyorsjavítás telepítésével megoldhatja a [problémát.](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d) 