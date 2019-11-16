---
title: ugyanaz mint filenév van legjobb
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800047"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Kötelező Alchemy fejléc H1, H2's nem működik.
A legjobb gyakorlatok és iránymutatások Alchemy authoring:

1. Ne **fészkel alkímia Insights a mappák**-Ez megtöri az URL struktúrát. Mi vagyunk látszó-ba rögzítő ez.
1. Az **Alchemyinsights** mappában lévő fájloknak kisbetűs fájlnevekkel kell rendelkezniük, a szóközök pl. kötőjelet kell tükrözniük. ***hogyan kell-Enable-perek-Hold***.
    1. A Rule ID, vagy a Bucket ID azonosítót az [alkímia partner portálja](https://alchemyportal.azurewebsites.net) tartalmazza a MS. Custom mezőben. Ex. ***MS. Custom: 100021***
1. Sablonként használhatja a fájl tetején lévő többi metaadatot.
1. Az [alkímia partner portálon](https://alchemyportal.azurewebsites.net), navigálni le a szakaszt **ügyfél Insight cím:** és használni, hogy a kiindulási pont a H1 címét a betekintést. 
    > [!NOTE]
    > Alchemy Insights kell lennie csak egy H1 a tetején, vagy fognak törni a termelést. H2s nem teszik sem így használja **merész** vagy más egyezmények jelzi külön szakaszok.
1. Következő, töltse ki a szövegtörzs segítségével a tervezet anyagot az ügyfél Insights szakaszában az alkímia szabály oldal
    1. A felsorolásjeles listák jól
    1. Számozott listák is
    1. **Félkövér** és *dőlt* is a-ok
    1. Linkek mindig vagy **"linkeket web"/külső** vagy **mély-linkek UI elemek**, nem a belső linkek.
    1. Képek nem hivatalosan támogatott ebben az időben, de ez az ütemterv.

És ez tényleg már egy kicsit túl hosszú. A legjobb gyakorlat mintegy 400 karakter---------------------------------

Egyszer-a elégedett van kész, húz ez-hoz él ág. Ezután menj az [alkímia partner portálra](https://alchemyportal.azurewebsites.net) és írd be a fájlnevet az URL mezőbe. 