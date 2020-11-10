---
title: OneDrive bejelentkezési hiba AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982480"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive bejelentkezési hiba AADSTS50011

Ha hibaüzenet jelenik meg a "AADSTS50011: a kérésben megadott válasz URL-címe nem egyezik meg" üzenettel a OneDrive alkalmazásba való bejelentkezéskor, ellenőrizze az alábbiakat:

A OneDrive-verziónak a 20.052. XXXX verzióval egyenlőnek vagy nagyobbnak kell lennie. XXXX. A verzió ellenőrzéséhez kattintson a kék OneDrive ikonra az értesítési területen, válassza a **súgó & a beállítások > a beállítások >** a beállítások lehetőséget.

A hálózat blokkolhatja a **g.Live.com** és a **oneclient.SFX.MS** való forgalmat. Ha a forgalom le van tiltva, a OneDrive nem tudja frissíteni magát. A hálózati rendszergazda segítségével gondoskodhat arról, hogy hozzáférhessen az URL-címekhez. [Ezek a végpontok](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) elérhetők a Microsoft 365-csomagokat használó ügyfelek számára.

Ha kézzel kell beszereznie a OneDrive aktuális verzióját, keresse fel [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
