---
title: Webhelyfeltárás
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030760"
---
# <a name="do-site-discovery"></a>Webhelyfeltárás

Ha szervezete továbbra is használja a régi webalkalmazásokat, és az Internet Explorer módot tervezi használni (amit a legtöbb ügyfél használ), akkor érdemes némi további webhelyfeltárási funkciókat is használnia.

**Már üzembe helyezett egy régebbi verziójú Microsoft Edge**

Ha már konfigurálta a vállalati webhelylistát az Microsoft Edge régi verziójára, akkor a webhelyfeltárás már majdnem kész. Az egyetlen dolog, amit érdemes megtennie, az, hogy semleges webhelyeket ad hozzá.

A semleges webhelyek általában egyszeri bejelentkezést (SSO) biztosítanak. Ha egy semleges webhelyet hoz Microsoft Edge, akkor a hitelesítéshez maradjon Microsoft Edge webhelyen. Ha az Internet Explorer módban semleges webhelyre vált, a hitelesítéshez az Internet Explorer módban szeretne maradni.

Azonosítsa az Ön által használt SSO- vagy egyéb semleges webhelyeket, és vegye fel őket a vállalati webhely listájára.

**Az Internet Explorer az alapértelmezett böngésző**

Ha most csak az Internet Explorert használja, nem biztos, hogy tudja, hogy mely webhelyek frissítettek modern webes szabványokra, és melyikhez még szükség van az Internet Explorerre. Ezeket a webhelyeket meg kell találnia és hozzá kell adni a vállalati webhelylistához, hogy csak az ezekre a webhelyekre tudjon Internet Explorer módot használni.

> [!NOTE]
> [A vállalati webhelyfeltárás](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) olyan webhelyeket fedez fel, amelyekhez szükség lehet az Internet Explorer módra. Adatokat gyűjthet az Internet Explorer 8-Windows Internet Explorer 11-ig Windows 10, Windows 8.1 vagy Windows 7 böngészőn keresztül.

**Az adatok elemzése**

Miután összegyűjtötte a webhelyadatokat, azt javasoljuk, hogy az alábbi négylépéses folyamattal elemezze az adatokat:
1. Rendezheti az adatokat tartomány, majd URL-cím szerint.
2. Határozza meg az Internet Explorer módban konfigurálni szükséges alkalmazások határait. Az appot definiáló összes webhelyet és webes vezérlőt szerepeletni szeretné, de nem szeretne további webhelyeket és vezérlőket szerepeletni. Egyes webhelyek lehetnek olyan egyszerűek, mint amikor mások több webhely és lap *https://contoso.com/app1* definiálát követelik meg Öntől.
3. Tesztelje az appot, és ellenőrizze, hogy nem működik-e natív módon. Sok webhely kínál modern tartalmat, ha modern böngészőt észlel, és csak a régi tartalmakat, amikor az Internet Explorert észleli.
4. Ha nem sikerül a tesztelés, vegye fel az alkalmazást a vállalati webhelylistára.

> [!NOTE]
> Ajánlott eljárásként csoportosítsa az appot magában foglaló összes webhelyet. Ily módon az alkalmazások frissítések frissítésekjében egyszerűbben eltávolíthatja a teljes webhelyet az Internet Explorer módból, és egy modern böngészőt kezdhet az alkalmazáshoz.

Ha végzett a webhely felfedezésével, és elemezte az adatokat, készen áll a csatornastratégia elemzésére.

