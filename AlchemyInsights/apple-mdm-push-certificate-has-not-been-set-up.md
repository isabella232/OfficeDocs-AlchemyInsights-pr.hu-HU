---
title: Az Apple MDM leküldéses tanúsítványa nincs beállítva
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439382"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Az Apple MDM leküldéses tanúsítványa nincs beállítva

Az Apple MDM leküldéses tanúsítványa (más néven Apple Push Notification Service (APNS) tanúsítvány) nincs konfigurálva az előfizetéshez. Az Apple MDM leküldéses tanúsítványkonfigurálása nélkül nem tud iOS és Mac OS-eszközöket beállítani és kezelni. Miután hozzáadja a tanúsítványt az Intune-hoz, a felhasználók telepíthetik a Céges portál alkalmazást az iOS-eszközök regisztrálásához.

1. Válassza az **"Egyetértek" lehetőséget.** hogy a Microsoft engedélyt adjon az Apple-nek küldött adatok küldésére.

2. Válassza **az CSR letöltése** lehetőséget az Apple MDM leküldéses tanúsítvány létrehozásához szükséges Intune-tanúsítvány-aláíró kérelemre. A fájl segítségével megbízhatósági kapcsolattanúsítványt kérhet az Apple Push Certificates Portal-tól.

3. Válassza **az MDM leküldéses tanúsítvány létrehozása lehetőséget** az Apple Push Certificates Portal megugrásához. Jelentkezzen be a cégével, az Apple ID azonosítóval, és válassza **a Tanúsítvány létrehozása lehetőséget.** Válassza **a Fájl kiválasztása**lehetőséget, keresse meg a tanúsítványaláíró kérelemfájlt, majd válassza a **Feltöltés gombot.** A Megerősítés lapon válassza a **Letöltés** gombot a tanúsítványfájl (.pem) letöltéséhez, majd a fájl helyi mentéséhez.
 
**Megjegyzés:** A tanúsítvány a létrehozásához használt Apple ID azonosítóhoz van társítva. Ajánlott eljárásként használjon vállalati Apple ID azonosítót a felügyeleti feladatokhoz, és győződjön meg arról, hogy a postaládát egynél több személy vagy terjesztési lista használatával figyeli. Soha ne használjon személyes Apple ID azonosítót. Használja ugyanazt az Apple ID azonosítót az Apple Push tanúsítvány 12 havonta történő megújításához.
 
4. Adja meg az Apple MDM leküldéses tanúsítvány létrehozásához használt Apple ID azonosítót. Rögzítse ezt az azonosítót emlékeztetőként, amikor meg kell újítania a tanúsítványt.

5. Nyissa meg a tanúsítványfájlt (.pem), válassza **a Megnyitás**lehetőséget, és válassza **a Feltöltés gombot.** A leküldéses tanúsítvánnyal az Intune regisztrálhatja és kezelheti az Apple-eszközöket.