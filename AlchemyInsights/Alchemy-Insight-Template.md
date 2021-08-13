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
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918897"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Kötelező Alchemy-fejléc H1, a H2-es nem működik."
Ajánlott eljárások és útmutatás az Alchemy-íráshoz:

1. **Ne ágyazhatja be az Alchemy Elemzések** mappákba – ez megszakítja az URL-struktúrát. Javítani szeretnénk a probléma megoldását.
1. Az **AlchemyInsights** mappában lévő fájloknak kisbetűs, kötőjelekkel elválasztott fájlneveket kell tartalmazni a szóközök számára. **_how-to-enable-litigation-hold._**
    1. Az ms.custom mezőbe az [Alchemy-partnerportálról](https://alchemyportal.azurewebsites.net) származó szabályazonosítót vagy gyűjtőazonosítót is fel kell foglalni. pl. ***ms.custom: 100021***
1. A fájl tetején lévő többi metaadatot használja sablonként.
1. Az [Alchemy](https://alchemyportal.azurewebsites.net)Partnerportálon lépjen a **Customer Insight Title (Ügyféladatok címe)** szakaszra, és használja ezt kiindulási pontként az 1. h1-es címhez a betekintéshez. 
    > [!NOTE]
    > Az Alchemy Elemzések A gép tetején csak egyetlen H1 számnak kell lennie, különben meg fog szakítani a gyártást. A H2s sem jelenik  meg, ezért használjon félkövér vagy más konvenciót az egyes szakaszok jelzésére.
1. Ezután töltse ki a törzsszöveget az Alchemy-szabály Customer Insights szakaszának vázlatával.
    1. A listajeles felsorolások rendben vannak
    1. Számolt listák is
    1. **A** *félkövér és* a dőlt formázás rendben van
    1. A hivatkozásoknak mindig **"webes"/külső** **VAGY** mélyhivatkozásnak kell lennie a felhasználói felület elemeire, nem pedig belső hivatkozásoknak.
    1. A képek jelenleg hivatalosan nem támogatottak, de a fejlesztési ütemtervben szerepel.

És ez már egy kicsit túl hosszú. Ajánlott körülbelül 400 karakterből ---------------------------------

Ha elkészült a tartalom, húzza át az élő ágba. Ezután lépjen az [Alchemy Partner portálra,](https://alchemyportal.azurewebsites.net) és írja be a fájlnevet az URL-mezőbe. 