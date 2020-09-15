---
title: ugyanaz, mint a fájlnév a legjobb
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664136"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"A kötelező alkímia fejléce, a H2's nem működik."
Ajánlott eljárások és útmutatók az alkímia szerkesztéséhez:

1. Ne **ágyazza be az Alchemy**-elemzéseket a mappákba – Ez megtöri az URL-struktúrát. Ebben a cikkben keresünk.
1. A **AlchemyInsights** mappában lévő fájloknak kisbetűs fájlnevet kell használniuk az ex szóköz billentyűkombinációval. ***útmutató – engedélyezés – peres eljárás***
    1. Adja meg a szabály AZONOSÍTÓját vagy a vödör AZONOSÍTÓját az [Alchemy partner portálról](https://alchemyportal.azurewebsites.net) a MS. egyéni mezőben. ex. ***MS. Custom: 100021***
1. Használja a fájl felső részén található metaadatokat sablonként.
1. Az [Alchemy partner portálon](https://alchemyportal.azurewebsites.net)lépjen lefelé az **ügyfél-betekintési cím** mezőbe, és használja azt kiindulási pontként az Insight-címéhez. 
    > [!NOTE]
    > Az alkímiai elemzéseknek csak egy H1-nek kell lenniük a tetején, vagy a termelésben szünetük lesz. A H2s nem jeleníti meg a **félkövér** vagy más konvenciókat, hogy külön szakaszt adjon meg.
1. Ezután töltse ki a szövegtörzset az Alchemy szabály lapjának ügyfél-betekintési részén található anyag segítségével.
    1. A listajeles felsorolások jól láthatók
    1. Számozott listák
    1. A **félkövér** és a *dőlt* a-ok
    1. A hivatkozásoknak mindig a **"hivatkozások a webre"/External** kell lenniük, vagy **mély hivatkozásokat kell használniuk a felhasználóifelület-elemekre, nem pedig a**belső hivatkozásokra.
    1. Jelenleg a képek jelenleg nem támogatottak, de az ütemterven van.

És ez már egy kicsit túl hosszú. A helyes gyakorlat a 400 karakterekről szól---------------------------------

Miután elkészült a tartalom, húzza azt az aktív ágra. Ezután nyissa meg az [Alchemy Partner portált](https://alchemyportal.azurewebsites.net) , és írja be a fájlnevet az URL-mezőbe. 