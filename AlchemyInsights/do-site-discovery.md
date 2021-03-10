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
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693486"
---
# <a name="do-site-discovery"></a>Webhelyfeltárás

Ha a szervezete továbbra is régi webalkalmazásokat használ, és az Internet Explorer módot tervezi használni (amelyet a legtöbb ügyfél használ), akkor további webhelyfeltárási lehetőségeket kell használnia.

**Már telepítette a Microsoft Edge egy régebbi verzióját**

Ha már beállította a vállalati webhelylistát a Microsoft Edge régi verziójának megfelelőre, akkor a webhelyfeltárás már majdnem kész. Az egyetlen dolog, amit érdemes lehet megtennie, hogy semleges webhelyeket ad hozzá.

A semleges webhelyek általában egyszeri bejelentkezést biztosítanak. Ha a Microsoft Edge-től egy semleges webhelyre kerül, a hitelesítéshez a Microsoft Edge-ben szeretne maradni. Ha az Internet Explorer módban semleges webhelyre vált, a hitelesítéshez az Internet Explorer módban szeretne maradni.

Azonosítsa az Ön által használt SSO- vagy egyéb semleges webhelyeket, és vegye fel őket a vállalati webhelylistára.

**Az Internet Explorer az alapértelmezett böngésző**

Ha most csak az Internet Explorert használja, nem biztos, hogy tudja, hogy mely webhelyek frissítettek modern webes szabványokra, és melyekhez még szükség van az Internet Explorerre. Ezeket a webhelyeket meg kell találnia, és hozzá kell adnia a vállalati webhelylistához, hogy csak az ilyen webhelyekhez tudja használni az Internet Explorer módot.

> [!NOTE]
> [A Vállalati webhelyfeltárás](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) feltárja az Internet Explorer módra esetleg szüksége lehet a webhelyeket. Adatokat gyűjthet Windows Internet Explorer 8–Internet Explorer 11 rendszerű számítógépeken Windows 10, Windows 8.1 vagy Windows 7 rendszeren.

**Az adatok elemzése**

Miután összegyűjtötte a webhelyadatokat, az adatok elemzéséhez az alábbi négylépéses eljárást javasoljuk:
1. Rendezheti az adatokat tartomány, majd URL-cím szerint.
2. Adja meg az Internet Explorer módban konfigurálni szükséges alkalmazáshatárokat. Az appot definiáló összes webhelyet és webes vezérlőt fel szeretné azonbanni, de nem szeretne további webhelyeket és vezérlőket tartalmazni. Egyes webhelyek lehetnek olyan egyszerűek, mint amikor mások több webhely és lap *https://contoso.com/app1* definiálását követelik meg.
3. Tesztelje az alkalmazást annak ellenőrzéséhez, hogy nem működik-e natív módon. Sok webhely kínál modern tartalmakat, amikor modern böngészőt észlel, és csak régi tartalmakat ajánl fel, amikor az Internet Explorert észleli.
4. Vegye fel az appot a vállalati webhelylistára, ha nem tudja tesztelni.

> [!NOTE]
> Gyakorlati megoldásként csoportosítsa az appot magában foglaló összes webhelyet. Ily módon az appok frissítésekkor egyszerűbben távolíthatja el a teljes webhelyet az Internet Explorer módból, és elkezdheti használni az app modern böngészőjét.

Ha végzett a webhelyfeltárással, és elemezte az adatokat, készen áll a csatornastratégia elemzésére.

