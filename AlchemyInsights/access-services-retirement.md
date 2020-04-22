---
title: Hozzáférés szolgáltatások nyugdíjazás
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687260"
---
# <a name="access-services-retirement"></a>Hozzáférés szolgáltatások nyugdíjazás

Ahogy azt eredetileg az MC97576-ban, 2017 márciusában jelentettük be, és az elmúlt évben folytattuk a kommunikációt, az Access Services-t megszüntették. A folyamat következő fázisa az Access webadatbázisok eltávolítása lesz, amelyek a SharePoint-listákat használják alapul szolgáló adattárolóként.

**Milyen hatással van ez rám?**

2019 júniusátantól leállítjuk az új Access-adatbázisok létrehozását a SharePoint Online-ban, és 2020 áprilisáig leállítjuk a szolgáltatást és a többi alkalmazást.

**Mit kell tennem, hogy felkészüljek erre a változásra?**

Javasoljuk, hogy hozzon létre egy átmeneti tervet a szervezet Access webes adatbázisaihoz. A rendszergazdák a [SharePoint Access alkalmazásképolvasó](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) segítségével leltárt kaphatnak a webhelyek által használt Access-alkalmazásokról.

Az Access webes adatbázisok adatainak áttelepítése többféleképpen is elérhető:

- Importálás helyi Access adatbázisba (. ACCDB) vagy egy Excel-fájlba.
- Azt is javasoljuk, hogy vizsgálja meg a Microsoft PowerApps-et alternatív platformként, hogy kód nélküli üzleti megoldásokat hozzon létre webes és mobileszközökhöz.