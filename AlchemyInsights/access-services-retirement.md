---
title: Az Access Services nyugdíjazása
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
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698684"
---
# <a name="access-services-retirement"></a>Az Access Services nyugdíjazása

Ahogy azt eredetileg a MC97576-ban jelentették be, az 2017 márciusi verziójában továbbra is megszűnt a kommunikáció az elmúlt évi Access-szolgáltatásokkal. A folyamat következő fázisa azokat az Access-webadatbázisokat fogja eltávolítani, amelyek a SharePoint-listákat használják a mögöttes adattárolóként.

**Milyen hatással van ez rám?**

A 2019 júniusi verziójában az új Access-adatbázisok létrehozása megszűnik a SharePoint Online-ban, és április 2020-től leállíthatja a szolgáltatást és a fennmaradó alkalmazásokat.

**Mit kell tennem, hogy felkészüljenek erre a változásra?**

Javasoljuk, hogy hozzon létre egy áttűnési tervet a szervezete Access-alapú webes adatbázisaihoz. A rendszergazdák a [SharePoint Access app-szkenner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) segítségével beállíthatják a webhelyek által használt Access-alkalmazások leltárát.

Az Access-webadatbázisok adatainak áttelepítése többféle módon történik:

- Importálás helyi Access-adatbázisba (. ACCDB) vagy egy Excel-fájlra.
- Javasoljuk, hogy a Microsoft PowerApps-ot alternatív platformként vizsgálja meg, hogy a rendszer nem hoz létre a webes és mobileszközök számára a nem-kódolt üzleti megoldásokat.