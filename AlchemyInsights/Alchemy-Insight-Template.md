---
title: same as filename is best
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
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312827"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Kötelező Alchemy-fejléc H1, a H2-es nem működik."
Ajánlott eljárások és útmutatás az Alchemy-íráshoz:

1. **Ne ágyazhatja be az Alchemy Elemzések mappákba**– ez megszakítja az URL-struktúrát. Javítani szeretnénk a probléma megoldását.
1. Az **AlchemyInsights** mappában lévő fájloknak kisbetűs, kötőjelekkel elválasztott fájlneveket kell tartalmazni (például). **_how-to-enable-litigation-hold._**
    1. Az ms.custom mezőbe az [Alchemy-partnerportálról](https://alchemyportal.azurewebsites.net) származó szabályazonosítót vagy gyűjtőazonosítót is fel kell foglalni. pl. ***ms.custom: 100021***
1. A fájl tetején lévő többi metaadatot használja sablonként.
1. Az [Alchemy](https://alchemyportal.azurewebsites.net)Partnerportálon lépjen a **Customer Insight Title (Ügyféladatok címe)** szakaszra, és használja ezt kiindulási pontként az 1. h1-es címhez a betekintéshez. 

**Megjegyzés:** Az Alchemy Elemzések csak egyetlen H1 H1-et kell a képernyő tetején tartania, különben meg fog szakítani a gyártást. A H2s sem jelenik  meg, ezért használjon félkövér vagy más konvenciót a különálló szakaszok jelzésére.
1. Ezután töltse ki a törzsszöveget az Alchemy-szabály lap Customer Insights szakaszának vázlatával.
    1. A listajeles felsorolások rendben vannak
    1. Számolt listák is
    1. **A** *félkövér és* a dőlt formázás rendben van
    1. A hivatkozásoknak mindig **"webes"/külső** **VAGY** mélyhivatkozásnak kell lennie a felhasználói felület elemeire, nem pedig belső hivatkozásoknak.
    1. A képek jelenleg hivatalosan nem támogatottak, de a fejlesztési ütemtervben szerepel.

És ez már egy kicsit túl hosszú. Ajánlott körülbelül 400 karaktert ---------------------------------

Ha elkészült a tartalom, húzza át az élő ágba. Ezután lépjen az [Alchemy Partner portálra,](https://alchemyportal.azurewebsites.net) és írja be a fájlnevet az URL-mezőbe. 