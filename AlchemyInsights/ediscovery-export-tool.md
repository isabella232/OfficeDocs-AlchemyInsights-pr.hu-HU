---
title: eDiscovery export tool
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814590"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nem tudja telepíteni vagy futtatni az Elektronikus adatok exportálása eszközt?

Ha nem tudja telepíteni vagy futtatni az Elektronikus adatok exportálása eszközt a keresési eredmények letöltéséhez, ellenőrizze az alábbiakat:
  
- A használt számítógép megfelel az alábbi előfeltételeknek:

  - A Windows 7 és az újabb verziók 32 vagy 64 bites verziója

  - Microsoft .NET Framework 4.7

  - Támogatott böngésző:

  - Microsoft Edge

    Vagy

  - Internet Explorer 10 vagy újabb verziók

    Más böngészők, például a Google Chrome és a Mozilla Firefox nem támogatottak.

- Szervezete csatlakozhat az Azure-beli végponthoz, amely **\* .blob.core.windows.net** (a helyettesítő karakter az exportálási feladat egyedi azonosítóját jelöli).

- Exportálási szerepkört kap a Microsoft 365 Biztonsági megfelelőségi &amp; központban. Ez a szerepkör alapértelmezés szerint csak az Elektronikus észlelés-kezelő szerepkörcsoporthoz van hozzárendelve. Lásd: [Elektronikus észlelési engedélyek hozzárendelése.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

További információ: [Tartalomkeresés eredményeinek exportálása.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Ha több mint 100 000 000 postaládát exportál, a következő Powershell használatával kell letöltenie az Eredmények exportálása: Találatok exportálása több mint  [100 000 postaládából](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)parancsot.