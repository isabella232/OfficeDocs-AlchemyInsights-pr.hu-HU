---
title: Access services retirement
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938697"
---
# <a name="access-services-retirement"></a>Access services retirement

Ahogyan azt eredetileg az MC97576-ban bejelentettük 2017 márciusában, és az elmúlt egy év során folyamatosan kommunikáltunk, Access Services meg. A folyamat következő fázisa lesz a webes Access-adatbázisok eltávolítása, amelyek SharePoint listákat használják mögöttes adattárolásként.

**Milyen hatással van ez rám?**

2019. júniustól kezdődően leállítjuk az új Access-adatbázisok létrehozását az SharePoint Online-ban, és 2020 áprilisáig leállítjuk a szolgáltatást és a többi appot.

**Mit kell tennem a változásra való felkészüléshez?**

Azt javasoljuk, hogy hozzon létre egy áttérési tervet a szervezet webes Access-adatbázisai számára. A rendszergazdák az Access [SharePoint alkalmazásolvasóval](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) lek minderől lekértetik a webhelyeken használt Access-appok készletét.

A webes Access-adatbázisok adatainak áttelepítése többféleképpen is lehetséges:

- Importálás helyi Access-adatbázisba (. ACCDB) vagy egy Excel fájlba.
- Azt is javasoljuk, Microsoft PowerApps alternatív platformként a kód nélküli üzleti megoldások létrehozásához webes és mobileszközök számára.