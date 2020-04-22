---
title: ugyanaz, mint a fájlnév a legjobb
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676535"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Szükséges Alkímia Fejléc H1, H2's nem működik.
Gyakorlati tanácsok és irányelvek az alkímia iméniai szerkesztéshez:

1. **Ne ágyazd be az Alchemy Insights-ot a mappákba**- ez megtöri az URL-struktúrát. Ezt meg akarjuk javítani.
1. Az **AlchemyInsights** mappában lévő fájloknak kisbetűs fájlnevekkel kell rendelkezniük, kötőjelekkel az ex szóközökhöz. ***hogyan lehet engedélyezni a peres eljárásokat.***
    1. Adja meg a szabályazonosítót vagy a gyűjtőazonosítót az [Alkímiapartner portálról](https://alchemyportal.azurewebsites.net) az ms.custom mezőben. Ex. ***ms.custom: 100021***
1. Sablonként használja a fájl tetején lévő többi metaadatot.
1. Az [Alkímia partner portálján](https://alchemyportal.azurewebsites.net)keresse le az **Ügyfél betekintési címe szakaszt,** és használja ezt a H1 cím kiindulópontjaként az elemzéshez. 
    > [!NOTE]
    > Alchemy Insights kell csak egy H1 a tetején, vagy azok szünet a termelésben. A H2s nem teszi kitévá az okat, ezért **használjon félkövér** vagy más konvenciókat a különálló szakaszok jelzéséhez.
1. Ezután töltse ki a törzsszöveget az Alkímiai szabály lap Customer Insights szakaszában található vázlat anyag használatával.
    1. A listajeles listák rendben vannak
    1. Számozott listák is
    1. **Merész** és *dőlt* a-ok
    1. Linkek mindig vagy **"linkeket web"/ külső** VAGY **mély-linkeket ui elemek**, nem belső linkek.
    1. A képek hivatalosan nem támogatottak jelenleg, de az ütemtervben szerepelnek.

És ez már így is egy kicsit túl hosszú. Az ajánlott eljárás körülbelül 400 karakter ---------------------------------

Ha a tartalom készen áll, húzza ki az élő ágba. Ezután nyissa meg az [Alchemy Partner portált,](https://alchemyportal.azurewebsites.net) és írja be a fájlnevet az URL mezőbe. 