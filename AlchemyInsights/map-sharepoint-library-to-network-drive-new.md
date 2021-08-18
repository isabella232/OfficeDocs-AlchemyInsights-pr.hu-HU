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
ms.openlocfilehash: 4eae45992d3fe6b31ae4d1aed02484cf20cb2260
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315550"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>Tár SharePoint hálózati meghajtóhoz

Hálózati meghajtó megfeleltetése helyett szinkronizálja a SharePoint az új ügyfélalkalmazással OneDrive szinkronizálási app igény szerinti fájlokat biztosít. A OneDrive-ban lévő összes fájl elérése helyi tárterület használata nélkül. További információ: [Az](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) SharePoint-Teams-fájlok szinkronizálása a számítógéppel és Lemezterület megtakarítása az OneDrive Igény szerinti fájlok igény szerinti [Windows 10.](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)

Ha úgy dönt, hogy az új ügyfélprogram helyett egy meghajtót [OneDrive szinkronizálási app](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)meg, kövesse az alábbi lépéseket:

- [A SharePoint Online-hoz csatlakoztatott leképezett hálózati meghajtók hibáinak elhárítása](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [Hitelesítési hibák akkor fordulnak elő, ha az ügyfél nem támogatja a TLS 1.2-es használatát](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**MEGJEGYZÉS:** Ha a Internet Explorer 10-ot használja a Windows 8-es vagy Windows 7-es,  és a meghajtó megfeleltetésekor nem érhető el az **Access** megtagadva vagy az Elérési út nem érhető el, a gyorsjavítás telepítésével megoldhatja a [problémát.](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)